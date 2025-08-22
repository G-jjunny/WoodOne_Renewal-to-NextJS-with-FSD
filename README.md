

## ⚙️ 아키텍처: FSD (Feature-Sliced Design)
이 Nextjs 프로젝트는 FSD 아키텍처 기반으로 구성되었습니다. 
프론트엔드 프로젝트에서 관심사의 분리(Separation of Concern) 와 기능 중심의 모듈화(Modularization) 를 돕는 구조입니다.
FSD는 애플리케이션을 기능 단위로 분할하고, 각 기능을 독립적으로 개발, 테스트, 유지보수할 수 있도록 하는 것을 목표로 합니다.


```

├── app
│   └── about          # NextJS의 App Router용 폴더 (re-export)
│   └── ...
│
├── pages              # NextJS의 Pages Router용 폴더 (제거 예정)
│   └── README.md      # 
├── src
│   ├── app            # FSD의 app layer
│   ├── pages          # FSD의 pages layer
│   ├── widgets        
│   ├── entities
│   ├── features
│   └── shared

```

