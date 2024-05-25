
![Infrast 1111111111111111111111111111](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/281ef7c1-efd1-49f4-8be3-1fba795c5298)

 How to create a customer account
===============

===> Type in the search box ===> IAM
=========================

![1](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/abff00b5-ae6c-4aaa-ab43-603017b86f26)
![2](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/e1b91e04-700a-48fd-81c8-5a9bb17a7ba9)
![3](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/279b44fa-cf02-4b51-90d0-0eed9f24e408)
![4](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/15be7849-400a-4bc9-b40c-c9d251244736)
![5](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/82f553a5-1db7-48ea-a2a0-ccb7d675af4b)
![6](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/f18c723a-0a39-472e-bc3c-fa3ef7f508a3)


Let's Begin
Type in the search box
=====================
![VPC_1](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/53d5307e-7945-4341-8a05-5a0297ab1fce)
![VPC_2](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/5ed2b29f-5a29-4ebf-bf02-85bcc4908fe2)
![VPC_3-1](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/584dd0a1-876d-42d8-978b-d6356e0008fb)

Create subnets 
===========
Inside VPC to divide smaller blocks and separation
===================================
![VPC_3-2](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/0b4b1ba7-16e4-4c4f-a930-bb91dd1957a8)
![VPC-3-3](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/d647b65f-aef7-48bb-8cd2-3b5ae60c350a)
![VPC_3-4](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/72a37fa3-c08a-4586-b76e-00db368d5ea4)
![VPC_3-5](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/84fe0bb9-f1f9-43f8-8810-ab5ecdc2f4b5)

Create Internet gateway and 
-----------------------

![7](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/b4a83d61-7e3e-4bb5-aa7a-8ad4fc6720f7)

![8](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/1d4c2563-d1cf-46dd-be34-2d0eb08d7d3a)

attach to VPC
------------------
![9](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/5fefa625-3797-4b47-8a74-a22d7dc7e911)

![10](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/9a67ee95-4bda-4efb-b99f-92ea5a191985)

Create Virtual Private Gateway
----------------

Virtual Private network (VPN)   ==> Virtual Private Gateway
----------------
![11](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/6a9540d2-3a02-46a6-9a58-e1b0779eb910)
![12](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/0cbfb28b-a6c6-4a72-972d-fcd69dacc20a)


attach to VPC
------------------
![13](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/2a3e1cde-6d52-4514-9f0a-c00f4a494b17)

![14](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/3f8085f2-7796-4c44-820b-ba40d59f3a52)
![15](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/bc66bddf-49ad-4f0d-aa55-9a889b1dadd0)

Create route tables
------------------
![16](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/750d4bcd-62ba-412a-be94-bad50a4f7f38)
![17](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/66db68f6-4aad-4bca-b8a3-c41cc0c3d623)

![18](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/2f9aa178-426a-4b4a-9052-5aa47173ac7b)

One route for Internet gateway, another for Virtual private gateway (R1-IGW and R2-VGW)
------------------
Route - 0.0.0.0/0 to IGW
Route - 192.168.0.0/16 to VGW
------------------

Now edit R1-IGW and add routing rule as mentioned below
------------------

![19](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/cea7d3ce-9080-4c13-b03a-fbefa8eca4d9)
![20](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/7f2ca2a8-d47c-4e35-a7c3-6597e2bf4f7c)
![21](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/28561d92-8c77-4a44-b0bc-cee65bae7f00)

Now edit R2-VGW and add routing rule as mentioned below
------------------
![22](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/8f576b78-5a72-4d9d-baf9-a8b7a1d6902a)
![23](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/a35a030b-a4e0-4940-a46b-d24ad6efe300)
![24](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/300eef74-297a-40db-add1-a891482ca149)


Attach routing tables to subnets. R1-IGW to S3-Public and S4-Public, public network required to have internet access. 
Attach R2-VGW to S1-Private and S2-Private (No internet become a private subnets)
------------------

![25](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/755b0f91-219d-4c9c-9c59-c389d0a7899c)

![26](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/fb5be0f5-6feb-49db-99b7-f9b43a843920)

![27](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/d0b54440-ff12-4725-bffa-c14f4b726068)

![28](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/8029d48c-dfab-4922-9eb6-05c83090a68a)

![29](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/7abaaf4f-b057-4951-a9ab-83751db14f0e)
![30](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/d9432efd-d5da-43b9-93af-91ef060a527b)
![31](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/e19b6ca7-b2bb-4f87-b578-6ac22f25b754)
![32](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/9511e95e-ba92-4042-9dec-3862f084dae8)
![33](https://github.com/chalyouness/Foundations-of-Cloud-Computing/assets/114768920/154ca272-81d9-4e92-96f6-914cfc27367d)







