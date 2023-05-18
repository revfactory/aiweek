# AI-WEEK-02-PDF_Query_LLM

## :page_with_curl: 실습 파일 
### 전체 코드 :  [AI_WEEK_02_PDF_Query_LLM.ipynb](AI_WEEK_02_PDF_Query_LLM.ipynb)
### Colab Starter : https://colab.research.google.com/drive/1ROr4iRl4_vwUvDWCPBkc7haDmpWgyoi9?usp=sharing
- 사본을 만들어 코드를 완성해주세요!
- 실습용 [PDF 파일 다운로드](https://www.github.com/revfactory/aiweek/AI-WEEK-02-PDF_Query_LLM/raw/main/2023_GPT4All_Technical_Report.pdf) 

### OpenAI API 조별 실습용 키
- 별도 안내

 <br>
 
## :book: **실습 전 알아보기**  
### PDF 서비스 소개
- [ChatPDF](https://www.chatpdf.com)
### [LangChain](https://python.langchain.com/en/latest/index.html)
- [PyMuPDF](https://python.langchain.com/en/latest/modules/indexes/document_loaders/examples/pdf.html?highlight=PyMuPDF#using-pymupdf) : PDF 파일을 분석하고, 텍스트를 추출합니다.
- [CharacterTextSplitter](https://python.langchain.com/en/latest/modules/indexes/text_splitters/examples/character_text_splitter.html) : 텍스트를 분할합니다.
- [OpenAIEmbeddings](https://python.langchain.com/en/latest/modules/models/text_embedding/examples/openai.html?highlight=OpenAIEmbeddings) : OpenAI 의 임베딩을 적용합니다.
- [FAISS](https://python.langchain.com/en/latest/modules/indexes/vectorstores/examples/faiss.html?highlight=FAISS) : 효율적인 벡터 유사도를 구합니다.
- [Document Question Answering](https://python.langchain.com/en/latest/use_cases/question_answering.html?highlight=load_qa_chain#document-question-answering) : 질문과 유사도가 높은 여러 문서를 가져온 다음, LLM 을 통해 답변을 작성합니다.


### Hyper Parameter
- 온도(Temperature) 와 Top-p 설정은 모델이 응답을 생성할 때, 얼마나 결정론적인지 제어
- 정답이 하나만 있는 응답을 요청하는 경우 이 값을 낮게 설정
 <br>

## :dart: **전체 프로세스**  
- 이번 실습에서는 PDF 파일을 분석하고 추출된 텍스트와 Generative AI 를 이용하여 질문을 하는 과정을 살펴보려고 합니다.  
- 실습 전체 프로세스는 아래 그림과 같습니다.  

![image](https://github.com/revfactory/aiweek/assets/2889542/0dbce252-962f-4ff6-b3b8-09a4277a1bcf)


 <br>
 
## :pencil2: **참고링크**
- [LangChain](https://python.langchain.com/en/latest/index.html)
- [LangChain 을 알아볼까요?](https://revf.tistory.com/280)
- [LangChain 1,000만 달러 (130억) 시드 라운드 발표](https://blog.langchain.dev/announcing-our-10m-seed-round-led-by-benchmark/)
- [GPT-4 & LangChain - Create a ChatGPT Chatbot for Your PDF Files](https://github.com/mayooear/gpt4-pdf-chatbot-langchain)
- [Pinecone, 1억달러 시리즈B 펀딩 발표](https://www.pinecone.io/learn/series-b/)
