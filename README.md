# 유용한 북마크 관리, url 이미지 추출 익스텐션 ClipTab
> **GPT를 활용한 똑똑한 북마크와 URL 이미지 클립보드 활용**<br>


저희 서비스는 사용자가 **북마크를 통해 웹 페이지에 진입하기 전에** 간단한 정보를 확인할 수 있도록 **웹 페이지의 내용을 GPT로 요약**하여 제공하는 기능을 하는 **익스텐션**입니다. 그 뿐만 아니라, 특정 **URL에서 이미지를 추출하여 클립보드에 저장**하고 **활용**하는 기능도 함께 제공합니다.

<br>

## ❓What is Cliptab
**1.GPT를 통한 북마크 요약 제공**
```
1. 북마크 생성 시 해당 북마크의 url page 스크래핑
2. 스크래핑 된 data를 open api에게 넘기고 요약 정보 추출
3. 요약 정보를 저장했다가 사용자의 설정에 따라 제공
```
**2.북마크 알림 기능**
```
1. celery beat로 스케쥴링 된 task 실행
2. 알림이 필요한 북마크를 찾아 필요한 정보를 알림 테이블로 저장
3. 사용자가 확인하지 않은 알림이 있으면 아이콘 핑 처리
4. 아이콘 클릭 시 알림 페이지 제공
```
**3.클립보드를 활용한 url 이미지 활용**
```
1. url를 넣으면 해당 url page의 이미지 정보 스크래핑
2. 이미지(url)를 클립보드에 저장하고 drag&drop, download 등으로 활용
3. 새로 url을 넣으면 정해진 갯수를 넘어가는 데이터는 Queue 형식으로 자동 삭제 
```
<br>

## 🗂️Table of Contents

 - [Service Flow](#service-flow)
 - [Onboarding Page](#onboarding-page)
 - [System Architecture](#system-architecture)
 - [Tech Stack](#tech-stack)
 - [ERD](#erd)
 - [API](#api)
 - [Monitoring Tools](#monitoring-tools)
 - [Member](#member)
 - [Blog](#blog)

<br>

## 🔍Service Flow

<br>

## 📄Onboarding Page

<br>

## 🚧System Architecture


<br>

## 📚Tech Stack

| Frontend | Backend | DevOps | Monitoring | ETC |
|:--------:|:-------:|:------:|:----------:|:---:|
| <img src="https://img.shields.io/badge/React-61DAFB?style=flat&logo=React&logoColor=white"/><br><img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" /><br><img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" /><br><img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white" /><br><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=JavaScript&logoColor=white"/><br><img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=TypeScript&logoColor=white"/>| <img src="https://img.shields.io/badge/Django-092E20?style=flat&logo=Django&logoColor=white"/><br><img src="https://img.shields.io/badge/mysql-4479A1?style=flat&logo=mysql&logoColor=white"><br><img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white"><br><img src="https://img.shields.io/badge/Celery-37814A?style=flat&logo=celery&logoColor=white"> | <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=Docker&logoColor=white"/><br><img src="https://img.shields.io/badge/Amazon EC2-FF9900?style=flat&logo=Amazon EC2&logoColor=white"/><br><img src="https://img.shields.io/badge/Amazon RDS-527FFF?style=flat&logo=amazonrds&logoColor=white"/>| <img src="https://img.shields.io/badge/Grafana-F46800?style=flat&logo=Grafana&logoColor=white"/><br><img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=Prometheus&logoColor=white"/> | <img src="https://img.shields.io/badge/Slack-4A154B?style=flat&logo=Slack&logoColor=white"/><br><img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=Notion&logoColor=white"/><br><img src="https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=Postman&logoColor=white"/><br><img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=Swagger&logoColor=white"/><br><img src="https://img.shields.io/badge/GitHub Actions-2088FF?style=flat&logo=GitHub Actions&logoColor=white"/><br> |

<br>

## 🗄️ERD
<img width="924" alt="image" src="https://github.com/lsh1215/practice/assets/75378429/1aadd423-b3cb-425b-8463-ecfd5d7d5e83">

<br>

## 🔌API
<img width="1287" alt="image" src="https://github.com/lsh1215/practice/assets/75378429/591b746b-deaf-4a59-ab0d-4efbefee1f2a">
<img width="1288" alt="image" src="https://github.com/lsh1215/practice/assets/75378429/9d77fa48-748d-42ac-bc0f-57476a36911b">
<img width="1288" alt="image" src="https://github.com/lsh1215/practice/assets/75378429/f85993c0-6868-49ac-9eae-754616d1120e">
<img width="1288" alt="image" src="https://github.com/lsh1215/practice/assets/75378429/5d7dd03a-895f-454d-b1b8-641cd6f2abb1">


<br>

## 🖥️Monitoring Tools
> Prometheus & Grafana
> 

<br>

## 🙋🏻🙋Member
<table width="1000">
    <thead>
    </thead>
    <tbody>
    <tr>
        <th>Pictures</th>
         <td width="100" align="center">
            <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
             <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
             <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
             <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
             <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
        <td width="100" align="center">
            <a href="">
                <img src="" width="60" height="60">
            </a>
        </td>
    </tr>
    <tr>
        <th>Name</th>
        <td width="100" align="center">임아정</td>
        <td width="100" align="center">이민기</td>
        <td width="100" align="center">이주찬</td>
        <td width="100" align="center">소진수</td>
        <td width="100" align="center">박수빈</td>
        <td width="100" align="center">임동민</td>
        <td width="100" align="center">이상훈</td>
    </tr>
    <tr>
        <th>Position</th>
        <td width="150" align="center">
            Frontend<br>
            Leader<br>
        </td>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
        </td>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
        </td>
        <td width="150" align="center">
            Frontend<br>
        </td>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
        </td>
        <td width="150" align="center">
            Frontend<br>
        </td>
        <td width="150" align="center">
            Backend<br>
            DevOps<br>
        </td>
    </tr>
    <tr>
        <th>GitHub</th>
        <td width="100" align="center">
            <a href="https://github.com/Ajeong-Im">
                <img src="http://img.shields.io/badge/AjeongIm-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/kiminni">
                <img src="http://img.shields.io/badge/kiminni-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/JuChan-Lee">
                <img src="http://img.shields.io/badge/JuChanLee-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/thwlstn">
                <img src="http://img.shields.io/badge/thwlstn-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/suparb">
                <img src="http://img.shields.io/badge/suparb-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/dongmin115">
                <img src="http://img.shields.io/badge/dongmin115-green?style=social&logo=github"/>
            </a>
        </td>
        <td width="100" align="center">
            <a href="https://github.com/lsh1215">
                <img src="http://img.shields.io/badge/lsh1215-green?style=social&logo=github"/>
            </a>
        </td>
     </tr>
    </tbody>
</table>

<br>

## 📝Blog
