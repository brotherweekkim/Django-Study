# auto_now_add와 auto_now옵션의 차이

공식 문서: https://docs.djangoproject.com/en/1.10/ref/models/fields/#django.db.models.DateField

- 수정일자 : auto_now=True 사용
  auto_now=True 는 django model 이 save 될 때마다 현재날짜(date.today()) 로 갱신됩니다.
  주로 최종수정일자 field option 으로 주로 사용됩니다. 

- 생성일자 : auto_now_add=True 사용
  auto_now_add=True 는 django model 이 최초 저장(insert) 시에만 현재날짜(date.today()) 를 적용합니다.