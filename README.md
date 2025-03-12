
# 학사관리 시스템 (Education Management System)
 + 학생의 수강신청한 강의 목록을 조회하는 시스템

### 개발환경
  + Kotiln
  + Spring Boot
  + JPA
  + Thymeleaf
  + Gradle
  + MySQL
  + IntelliJ

# ERD 및 테이블 설계

![Image](https://github.com/user-attachments/assets/a714cea7-9d6a-4a77-ad68-e890ba3d97e6)

[ERD링크](https://www.erdcloud.com/d/4G4nwekLFbzPqW3zC)

+ 테이블 목록
  * student
   * taking classes
   * all the subjects
 
 ## 📋 **API**

### 👤 **수강과목 API**

| 기능            | 메서드   | 엔드포인트                       |
|-----------------|----------|----------------------------------|
| 수강과목전체조회  | `GET`   | `/studentAllinquiry/{studentnumber}`                     |
| 수강과목개별조회  | `GET`   | `/studentinquiry/{studentnumber}/{em_code}`                     |
| 수강과목삽입  | `POST`   | `/studentadd/{studentnumber}`                     |
| 수강과목수정    | `PUT`   | `/studentmodify/{studentnumber}`               |
| 수강과목삭제  | `DELETE`   | `/studentdel/{studentnumber}`              |

### 학생이 직접 수강과목을 수정하고 삭제할 수 있다.
#### 학생이 직접 관리하긴 애매한 부분이 있다 하지만 복잡하게 무엇을 더 추가하게 되면 미션 자체가 너무 어려워질 듯 하여, 가볍게 하기로 한다.
