날담 최종 통합 로그인/메모 버전

1. supabase-config.js에 기존 날담이 사용하던 Supabase Project URL 및 공개용 anon/publishable 키만 입력합니다. 비밀키는 절대 넣지 않습니다.
2. Supabase > Authentication > URL Configuration 에 https://abuzz85822021.github.io/naldam-web/ 를 Redirect URLs로 추가합니다.
3. Supabase > Authentication > Providers > Kakao 설정은 기존 프로젝트 그대로 유지합니다. Kakao Developers의 Redirect URI는 기존 Supabase 콜백 URI를 유지합니다.
4. 기존 memos 테이블의 RLS 정책이 authenticated 사용자 본인(user_id = auth.uid())에 대해 SELECT, INSERT, UPDATE, DELETE를 허용하는지 확인합니다. 기존 데이터를 삭제하거나 새 테이블을 생성하지 마세요.
5. 압축을 푼 파일을 naldam-web GitHub 저장소에 업로드하고 카카오 로그인 후 과거 메모 조회, 새 메모 저장, 로그아웃을 테스트합니다.

주의: 로그인은 기존 카카오 계정과 동일한 Supabase 프로젝트에서만 기존 사용자 ID 및 기록을 이어받습니다.
이 패키지는 기존 Render 앱이나 Supabase DB에 어떤 변경도 수행하지 않습니다.
