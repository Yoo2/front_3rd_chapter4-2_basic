# 바닐라 JS 프로젝트 성능 개선
- url: https://d7r50d538zjrn.cloudfront.net

## 성능 개선 보고서

### 초기
| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![초기](https://github.com/user-attachments/assets/69d33967-3652-474e-a986-019be3b61cda) | ![초기_2](https://github.com/user-attachments/assets/29e36d09-a954-420c-97f9-e98ce880b469) |

### 1번째 성능 최적화
![최적화1](https://github.com/user-attachments/assets/8d6a3dc9-168a-4eba-abbc-e5d4c80a59f7)

- jpg, png 확장자를 webp로 변경했습니다.

| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![최적화1_1](https://github.com/user-attachments/assets/7bbabb85-6f44-48f3-afbd-1b2d3af6c1ad) |![최적화1_2](https://github.com/user-attachments/assets/98b66f0c-7d4c-4734-867c-e62c2b00be1f)|
| 초기 대비 lcp 1.7초 감소 | 초기 대비 lcp 10.81초 감소 |

### 2번째 성능 최적화
![최적화2](https://github.com/user-attachments/assets/3e26d65a-ac83-4a02-b76e-d6f40bd2f8be)

- 글꼴을 웹에서 동적으로 받아오는 형식에서 정적파일로 받아오도록 변경했습니다.
- 히어로 이미지의 크기를 지정했습니다.

| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![최적화2_1](https://github.com/user-attachments/assets/177d229f-6409-4d4f-a6b0-5b842548f85a) |![최적화2_2](https://github.com/user-attachments/assets/7b8ca595-289b-4640-96db-f43ab9369060)|
| 최적화1 대비 fcp 0.2초, tbt 20밀리초, cls 0.5 감소 | 최적화1 대비 lcp 0.45 증가 |

### 3번째 성능 최적화
![최적화3](https://github.com/user-attachments/assets/aa24a033-fbb4-4b8f-b362-d823959312a9)

- media별로 다른 히어로 이미지를 렌더하도록 변경했습니다.

| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![최적화3_1](https://github.com/user-attachments/assets/9a0deee2-5d96-435d-a0c9-0414fac860e2) |![최적화3_2](https://github.com/user-attachments/assets/164ad5d9-6a7d-45ee-8ae8-2eb3a459a4e1)|
| 최적화2 대비 lcp 0.3초 tbt 140밀리초 증가 | 최적화2 대비 lcp 1.35 감소 |


### 4번째 성능 최적화
![최적화4](https://github.com/user-attachments/assets/31607df9-6827-4536-ae6e-58c2a6de860b)

- 웹 폰트 링크를 제거했습니다.

| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![최적화4_1](https://github.com/user-attachments/assets/99a8cac4-a586-4861-9e2e-59bb5c29854d) |![최적화4_2](https://github.com/user-attachments/assets/663e5272-721f-4f54-b39a-734a118c4cc7)|
| 최적화3 대비 lcp 0.4초 tbt 180밀리초 감소 | 최적화3 대비 lcp 0.11 증가 |

### 5번째 성능 최적화
![최적화5](https://github.com/user-attachments/assets/e5e368bb-3fbf-4721-b58a-dd34c175b606)

- 스크롤에 따라 product를 동적 로딩했습니다.

| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![최적화5_1](https://github.com/user-attachments/assets/9751cde6-b70d-4d0a-84f6-91f15d94ec66) |![최적화5_2](https://github.com/user-attachments/assets/8f2bd38d-6372-42a8-a514-05da4ad6a558)|
| 최적화4 대비 lcp 0.3초 tbt 200밀리초 감소 | 최적화4 대비 lcp 0.18 증가 |

### 6번째 성능 최적화
![최적화6](https://github.com/user-attachments/assets/ecaea575-3659-4850-a346-ea47eb1ac1ca)

- defer를 통해 script를 지연 로딩했습니다.

| PageSpeed Insights                                    | Lighthouse                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![최적화6_1](https://github.com/user-attachments/assets/691585b2-2004-4422-955c-b7df42d216ca) |![최적화6_2](https://github.com/user-attachments/assets/5b01027a-abb8-417d-a0f2-0ddac41fbe6c)|
| 최적화4 대비 fcp 0.2초 감소 | 최적화4 대비 lcp 1.03초 감소 |


### 최적화 Before & After

- PageSpeed Insights

| Before                                    | After                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![초기](https://github.com/user-attachments/assets/69d33967-3652-474e-a986-019be3b61cda) |![최적화6_1](https://github.com/user-attachments/assets/691585b2-2004-4422-955c-b7df42d216ca)|


- Lighthouse

| Before                                    | After                                                    |
| ------------------------------------- | ----------------------------------------------------- |
| ![초기_2](https://github.com/user-attachments/assets/29e36d09-a954-420c-97f9-e98ce880b469) |![최적화6_2](https://github.com/user-attachments/assets/5b01027a-abb8-417d-a0f2-0ddac41fbe6c)|
