# WepFramework2
# Homework3
Welcome to the helloSpringBoot wiki!

## 처음 테이블이 생성된 모습
![table](https://user-images.githubusercontent.com/52271770/85229112-ee697d80-b422-11ea-958c-2a05c3f2a8de.png)
<br><br>
## API method
1. Create/Add(Post) : create new product
![post](https://user-images.githubusercontent.com/52271770/85229139-1fe24900-b423-11ea-89c5-f813215f685e.png)
JSON형태로 Body에 담아 요청 -> Body 데이터를 데이터베이스에 생성(자동으로 ID할당)
<br><br>
2. Retrieve/Get (Get): <br>
   Get full list of products :
![getFullList](https://user-images.githubusercontent.com/52271770/85229166-56b85f00-b423-11ea-9217-50ff439ac572.png)
<br><br>
   Get details of products with id = N :
![getDetial](https://user-images.githubusercontent.com/52271770/85229177-63d54e00-b423-11ea-8a40-c0be10f9e626.png)
<br><br>
   Fetch all products of a category :
![fetchAllProducts](https://user-images.githubusercontent.com/52271770/85229202-73549700-b423-11ea-92bf-3deb37c9f517.png)
<br><br>
3. Update(PUT) : modify values of product with id = N 
![PUT](https://user-images.githubusercontent.com/52271770/85229228-823b4980-b423-11ea-95af-263b03731547.png)
url에 ID값을 넣어주고 JSON형태로 Body에 담아 요청 -> Body 데이터를 데이터베이스에 수정(url에 1번을 넣어줬기때문에 1번 정보인 MacBook 데이터에서 BossMonster 데이터로 수정됨)
<br><br>
4. Delete (DELETE) : delete product with id = N
![DELETE](https://user-images.githubusercontent.com/52271770/85229238-8ff0cf00-b423-11ea-931d-aeed267245bf.png)
정상 삭제 시 204 NO CONTENT가 호출되게 설정해놨기 때문에 204 NO CONTENT가 호출되어서 (ID : 11) 데이터가 정상 삭제 되었음을 알 수있음
<br><br>
<br><br>
## Spring Boot의 actuator를 활용하여 Products Rest API에 대한 URL Mapping 정보를 캡쳐해서 보여라.
![info](https://user-images.githubusercontent.com/52271770/85276244-7485d280-b4bc-11ea-851a-608d0450e392.png)

mappings 정보
![mappings](https://user-images.githubusercontent.com/52271770/85591613-64b6eb80-b680-11ea-8c77-aba9e10b1c8f.png)
# get mapping
![get1](https://user-images.githubusercontent.com/52271770/85590695-954a5580-b67f-11ea-9822-1c030d06883f.png)
![get2](https://user-images.githubusercontent.com/52271770/85590671-911e3800-b67f-11ea-83cf-318b4941e01e.png)
![get3](https://user-images.githubusercontent.com/52271770/85590666-8fed0b00-b67f-11ea-8e0e-ad968d77ac0b.png)

# delete mapping
![delete2](https://user-images.githubusercontent.com/52271770/85591328-2faa9900-b680-11ea-8255-766e5f27ac8c.png)
# post mapping
![post](https://user-images.githubusercontent.com/52271770/85590812-ae530680-b67f-11ea-98ab-1abc97227fe4.png)
# put mapping
![put](https://user-images.githubusercontent.com/52271770/85590582-7cda3b00-b67f-11ea-9441-5e391f52b0c8.png)
