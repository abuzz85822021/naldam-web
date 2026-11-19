날담 웹 버전 1차 미리보기

1. 이 폴더를 GitHub의 별도 공개 저장소(예: naldam-web)에 업로드합니다.
2. Settings > Pages > Deploy from a branch > main / (root) > Save를 선택합니다.
3. 발급된 GitHub Pages 주소에서 바로 열리는 달력, 한국사, 세계사, 계절 정보를 확인합니다.

주의: 기존 naldam-mobile 저장소와 Render 앱은 수정하지 마세요.
이것은 1차 미리보기로, 카카오 로그인/메모 저장, 음력, 공휴일, 절기, 천문 계산은 아직 구현하지 않았습니다.
로그인 연결 시에는 Supabase 프로젝트 URL 및 publishable/anon key만 브라우저에 사용하고, service_role key는 절대 올리지 마세요.
메모 접근에는 Supabase RLS가 반드시 설정되어 있어야 합니다.
