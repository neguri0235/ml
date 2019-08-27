### Google speech to text api 사용하기


##### 준비

1. Google Cloud 계정 만들기 (`https://cloud.google.com/speech-to-text/`)
2. Cloud Speech API 활성화 (`Cloud Speech Service Agent`)
3. json file을 local pc에 저장하기 - 환경 변수 설정 (`set GOOGLE_APPLICATION_CREDENTIALS=D:\@DevDocs\my-project-abc.json"`)
4. Google cloud sdk 설치 (https://cloud.google.com/sdk/docs/quickstart-windows)
5. `pip install google-cloud-speech` 설치
6. gcloud auth activate-service-account --key-file="D:\@DevDocs\my-project-abc.json" 를 통해 key 추가
7. `pip install pyaudio`
8. https://github.com/GoogleCloudPlatform/python-docs-samples/tree/master/speech/cloud-client 에서 sample source 받기
9. language code 변경
``` python
    language_code = 'en-US'  # a BCP-47 language tag
    language_code = 'ko-KR'  # a BCP-47 language tag
```
10. https://github.com/GoogleCloudPlatform/python-docs-samples/blob/master/speech/cloud-client/transcribe_streaming_mic.py 실시간 변환


참조: https://webnautes.tistory.com/1247