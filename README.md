# 개발자를 위한 ChatGPT 프롬프트 엔지니어링

[![Made with Jupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try) [![Made with python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

[강의][chatgpt-prompt-engineering-for-developers]에 등장하는 Jupyter Notebook 프롬프트들을 한국어로 다시 작성했습니다.

## Environment Variables

이 프로젝트를 실행하려면 .env 파일에 다음 환경 변수를 추가해야 합니다

`OPENAI_API_KEY`: [Open AI - API key](https://platform.openai.com/account/api-keys) 에서 API 키를 발급받아
사용하세요.

## Run Locally

프로젝트 클론

```bash
  git clone https://github.com/eunice-hong/deeplearning-ai-chatgpt-prompt-ko.git
```

프로젝트 위치로 이동

```bash
  cd deeplearning-ai-chatgpt-prompt-ko
```

필요한 라이브러리 설치

```bash
  pip install -r requirements.txt
```

Jupyter Notebook 실행

```bash
python -m notebook
```

## Lessons Learned

* 대화형 웹 인터페이스를 사용하는 것보다 Open AI API를 사용함으로써 훨씬 빠르고 정확하게 결과물을 얻을 수 있었다. 특히 원하는 결과물을 얻기 위해, 입력값을 다듬는
  과정이 비교적 간편했다. 대화형의 경우 일정 시간 이전의 기억을 유지시키기 위해, 대화 이전 입력값, 출력값을 중복해서 적시해야 했는데, API를 사용하는 경우 작성자가 세션을
  명시적으로 확인할 수 있어 입력값 정교화 과정에서 이전 기억을 번거롭게 입력할 필요가 사라졌다.
* 강의에서 사용한 형식 그대로 프롬프트를 한국어로만 번역해서는 LLM에서 원하는 결과물을 얻을 수 없다. 한국어로 자연스럽지 못한 명령어로 작성하는 경우, 원하는 조건을 충족하지
  못하거나 엉뚱한 결과를 받게 된다. 특히 화용론적 오류가 있는 지시를 주었을 때, 결과물을 영어로 출력해버리는 상황을 자주 마주했다. 따라서, 모국어라 하더라도 프롬프트 내용이
  명확한지
  검토해야만 한다.

## Feedback

질문/요청은 [Issue][project-issue]에 작성해주세요.

[project-issue]: https://github.com/eunice-hong/deeplearning-ai-chatgpt-prompt-ko/issues

## Related

- [SHORT COURSE - ChatGPT Prompt Engineering for Developers][chatgpt-prompt-engineering-for-developers]

[chatgpt-prompt-engineering-for-developers]: https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/

## Authors

- [@eunice-hong](https://www.github.com/eunice-hong)

