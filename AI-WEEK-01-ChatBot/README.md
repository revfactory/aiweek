# AI-WEEK-01-ChatBot

## :page_with_curl: 실습 파일 
### 전체 코드 : [AI_WEEK_01_ChatBot.ipynb](AI_WEEK_01_ChatBot.ipynb)
### Colab Starter : https://colab.research.google.com/drive/1vD557mlSnIPpl6cBE0s39sz2H-xzDNDG?usp=sharing
- 사본을 만들어 코드를 완성해주세요!

### OpenAI API 조별 실습용 키
- 별도 안내

 <br>

## :book: **실습 전 알아보기**  
### OpenAI API
- ChatGPT 무료에서 사용하는 것과 동일한 모델 사용 가능
- API KEY 발급은 [여기](https://platform.openai.com/account/api-keys) 에서 가능
- 아래와 같은 작업 가능
  - 이메일 또는 기타 글 초안 작성
  - Python 코드 작성
  - 일련의 문서에 대한 질문에 답변하기
  - 대화형 에이전트 만들기
  - 소프트웨어에 자연어 인터페이스 제공
  - 다양한 과목의 튜터
  - 언어 번역
  - 비디오 게임 등의 캐릭터 시뮬레이션


### gpt-3.5-turbo 모델
- 가격 : 1,000토큰 당 0.002달러로 기존 GPT-3.5 보다 10배 저렴
- URL : ```POST https://api.openai.com/v1/chat/completions``` 
- 입력 메세지는 메세지 객체의 배열이며, 각 메세지 객체는 역할과 내용으로 구성됩니다.
- 역할과 메세지
  - system : AI의 동작을 설정
  - user : 사용자가 작성한 메세지
  - assistant : AI가 작성한 메세지


### API 사용 예제
- Request
  ```python
  openai.ChatCompletion.create(
    model="gpt-3.5-turbo",
    messages=[
          {
            "role": "system", 
            "content": "You are a helpful assistant."
          },
          {
            "role": "user", 
            "content": "Who won the world series in 2020?"
          },
          {
            "role": "assistant", 
            "content": "The Los Angeles Dodgers won the World Series in 2020."
          },
          {
            "role": "user", 
            "content": "Where was it played?"
          }
      ]
  )
  ```
- Response
  ```python
  {
    'id': 'chatcmpl-6p9XYPYSTTRi0xEviKjjilqrWU2Ve',
    'object': 'chat.completion',
    'created': 1677649420,
    'model': 'gpt-3.5-turbo',
    'usage': {
      'prompt_tokens': 56, 
      'completion_tokens': 31, 
      'total_tokens': 87
    },
    'choices': [
      {
        'message': {
          'role': 'assistant',
          'content': 'The 2020 World Series was played in Arlington, Texas at the Globe Life Field, which was the new home stadium for the Texas Rangers.'
        },
        'finish_reason': 'stop',
        'index': 0
      }
    ]
  }
  ```


 <br>
 
## :pencil2: **참고링크**
- [OpenAI - Chat API Reference](https://platform.openai.com/docs/api-reference/chat)
- [OpenAI - Chat completions](https://platform.openai.com/docs/guides/chat)
- [프롬프트 모음: https://prompts.chat/](https://prompts.chat/)
- https://beta.character.ai/

