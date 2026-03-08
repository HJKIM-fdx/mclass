pipeline {
    agent any // 모든 서버에서 실행가능
    
    tools {
        maven 'maven 3.9.12'
        // Jenkins에 등록된 Maven 사용
    }


    environment {
        // 배포에 필요한 변수 설정
        DOCKER_IMAGE = "demo-app" // 도커 이미지 이름
        CONTAINER_NAME = "springboot-container" // 도커 컨테이너 이름
        JAR_FILE_NAME = "app.jar" // 복사할 JAR 파일 이름
        PORT = "8081" // 컨테이너와 연결할 포트
        REMOTE_USER = "ec2-user" // 원격(spring) 서버 사용자
        REMOTE_HOST = "174.129.229.212" // 원격(spring) 서버 IP (Public IP)
        REMOTE_DIR = "/home/ec2-user/deploy" // 원격 서버에 파일 복사할 경로
        SSH_CREDENTIALS_ID = "8f80f835-04e8-475c-88b0-70710a778aa4" // Jenkins SSH 자격 증명 ID
    }

    // 여러 단계를 그룹화
    stages {

    }

}