# UTS-Sistem Administrasi Server
------
## Rifqi Naufal Amanullah 1202190012    IT0201
------
**Question**
1. Download ISO Installer windows server 2022 a. https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022

2. Buat sebuah dokumentasi instalasi di github yang berisi

        a. Instalasi windows server 2022

        b. Instalasi Active Directory Domain Services

        c. Instalasi DNS server

        d. Instalasi Net Framework 3.5

        e. Promote Server to a Domain Controller

3. Kriteria Pengerjaan

        a. Dokumentasi pada github dengan format markdown

        b. Memberikan penjelasan beserta screenshoot Langkah Langkah instalasi

        c. Cukup mengerjakan poin no 2.A

        d. Poin no 2-B sampai 2-E boleh dikerjakan, nilai dari poin no 2-B sampai 2-E bisa mengatrol nilai praktikum atau nilai UAS.

**Answer**
------
### A. Instalasi windows server 2022
Download ISO Installer windows server 2022

   https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022
   
   Select download the `ISO` then follow it step by step.
 ![image](https://user-images.githubusercontent.com/93064971/143679628-f3759bee-40e0-46c7-81c1-9b4ceffe02f2.png)

- open `Oracle VM`, then Click `New` and Enter the name of the machine and type of system to use

![image](https://user-images.githubusercontent.com/93064971/143679686-8252c4df-5e91-45cb-b7c2-8157fb525154.png)
![image](https://user-images.githubusercontent.com/93064971/143679741-2ed83c15-4b2f-470c-94f6-cf30d5349286.png)

- Define the RAM, create the disk defining type and size

![image](https://user-images.githubusercontent.com/93064971/143679823-a787cc35-e798-4363-b9b3-b433e30ca381.png)
![image](https://user-images.githubusercontent.com/93064971/143679852-55472e9f-60bd-4510-b42d-156abebc5b2c.png)
![image](https://user-images.githubusercontent.com/93064971/143679869-f82a2546-9fe4-452a-b760-edb651ba01f0.png)
![image](https://user-images.githubusercontent.com/93064971/143679889-228a0af8-629d-4774-b684-a1dfc82b3120.png)
![image](https://user-images.githubusercontent.com/93064971/143679923-cbbbb40a-5fea-4773-b99c-35bdf96f141b.png)

- Go to the machine configuration and in the `Network` section set `Bridge adapter`

![image](https://user-images.githubusercontent.com/93064971/143679953-0f49e561-0311-41a8-a771-ee4a472be51d.png)

-  Click on `Start` and select the `ISO downloaded`

![image](https://user-images.githubusercontent.com/93064971/143680019-042803c2-83b0-4db1-b3b1-4d7cb2badf45.png)

-  Click on `Start` and the Windows Server 2022 installation wizard will load

![image](https://user-images.githubusercontent.com/93064971/143680032-9db4699c-74fa-4884-9423-139a9f4b867b.png)
![image](https://user-images.githubusercontent.com/93064971/143680046-fa78f913-61d3-425a-9ac6-6b413f3bd3f4.png)

-  Click on `Install now`

![image](https://user-images.githubusercontent.com/93064971/143680052-1c1cc06a-923c-4823-b0a7-3b6942c29477.png)

- Select windows server 2022 desktop experience
![image](https://user-images.githubusercontent.com/93064971/143680089-5ccc8e74-c59a-4440-b441-3615f22f0adb.png)

- Accept the license and then proceed with the installation of Windows Server 2022

![image](https://user-images.githubusercontent.com/93064971/143680110-8a54077c-e2cf-4048-87b7-5dc2a2335920.png)

- Select windows server 2022 install microsoft server advanced (Custom)

![image](https://user-images.githubusercontent.com/93064971/143680128-5ba070a2-a306-4919-9311-657a34b51eb7.png)

- Location installation of windows server 2022

![image](https://user-images.githubusercontent.com/93064971/143680141-2c4998c3-fa76-4465-86c1-0b0233912700.png)

- installation progress

![image](https://user-images.githubusercontent.com/93064971/143680155-5a0a4046-2f80-443f-abb4-3daf6ce5bacd.png)

- Next, custom your password administrator
![image](https://user-images.githubusercontent.com/93064971/143683163-5f93c249-269b-412d-88fe-018950318a2c.png)

- Access the menu `Input – Keyboard – Insert Ctrl + Alt + Del`. Enter the password created and wait for the configuration to load
![2021-11-27 (7)](https://user-images.githubusercontent.com/93064971/143683211-3d6d8f9a-ec88-4af5-a6b9-3d491463cb41.png)
![2021-11-27 (11)](https://user-images.githubusercontent.com/93064971/143683213-3257827f-d418-4c59-876f-7ea5e56d6c44.png)

```
- Windows Server 2022 has been successfully installed
```

### B. Instalasi Active Directory Domain Services
-  Before doing the installation, we change the computer name first by going to windows powershell.
   Then type `rename-computer -Newname Server2022`
    - Open the start menu and select `Windows PowerShell`
    ![2021-11-27](https://user-images.githubusercontent.com/93064971/143680317-558a5359-fee6-47e3-a71d-e5457e851809.png)
    ![2021-11-27 (1)](https://user-images.githubusercontent.com/93064971/143680443-751e7129-047f-420f-b3e7-9b1e815691be.png)
```
Then Restart, and open`Server Manager` 
```
- Select Menu `manage`, Then `Add Rules and Features` 
![2021-11-27 (2)](https://user-images.githubusercontent.com/93064971/143680344-f47e1d37-f2c9-48cd-9f49-2749d820e1ed.png)


- Select Next
![2021-11-27 (12)](https://user-images.githubusercontent.com/93064971/143680477-8233204f-6bc9-4e6b-b50a-a76db08c3a7e.png)

- Select option`Role-based or feature-based installation`. And `Next`
![WhatsApp Image 2021-11-27 at 11 02 36 PM](https://user-images.githubusercontent.com/93064971/143688529-d08754d9-8ddc-4e7b-9a14-142b7cfb6322.jpeg)


- Click `Select a server from the server pool` to select a local storage directory. Then `Next`
![WhatsApp Image 2021-11-27 at 11 02 38 PM](https://user-images.githubusercontent.com/93064971/143688546-c0ec75a6-55aa-4162-9bc5-1c5ffdedd99e.jpeg)

- Next, put a check mark in the `Active Directory Domain Services` box. When you check the box, on the right appears 
  a brief description of ADDS and how it works. Then click `Add Features`.
![2021-11-27 (17)](https://user-images.githubusercontent.com/93064971/143680933-81f4c0b8-85fd-4387-9019-4dd1e1f1a0ea.png)

### C. Instalasi DNS server
- We need to install and configure the Active Directory role and DNS server to work together.
  Checklist `DNS Servers` then `add features` 
![2021-11-27 (19)](https://user-images.githubusercontent.com/93064971/143688626-ac0ebbdb-c1a8-4704-b720-aec0175c0008.png)

### D. Instalasi Net Framework 3.5
- Checklist `.NET Framework 3.5 features`
![2021-11-27 (20)](https://user-images.githubusercontent.com/93064971/143680982-131034d7-a001-4a74-9721-32594958dd59.png)

- Click `Next`
![2021-11-27 (21)](https://user-images.githubusercontent.com/93064971/143680997-2bd7b3c6-30dc-4776-867d-997fa0f6838b.png)
![2021-11-27 (22)](https://user-images.githubusercontent.com/93064971/143681004-dd3c2923-f403-406b-a1f8-0b8ae645df14.png)

- Select `Install`
![2021-11-27 (23)](https://user-images.githubusercontent.com/93064971/143681024-bdae2d12-9245-46d1-bcc0-ed3f4dde3654.png)
![2021-11-27 (24)](https://user-images.githubusercontent.com/93064971/143681025-c45e5b7d-aaf1-45f0-b31a-922cbc40fd86.png)

### E. Promote Server to a Domain Controller
-  Setting to static ip using `cmd`, type `sconfig`

![WhatsApp Image 2021-11-27 at 11 02 45 PM](https://user-images.githubusercontent.com/93064971/143688660-9e09e8c4-020e-4603-91a9-a1b34a4b2fab.jpeg)

![WhatsApp Image 2021-11-27 at 11 02 47 PM](https://user-images.githubusercontent.com/93064971/143688676-8ee52b5c-434c-42b2-88d2-645becfa98a0.jpeg)

![WhatsApp Image 2021-11-27 at 11 02 47 PM (1)](https://user-images.githubusercontent.com/93064971/143688681-8ea6b35a-e209-48da-8848-bfe0583933d3.jpeg)

![WhatsApp Image 2021-11-27 at 11 02 47 PM (2)](https://user-images.githubusercontent.com/93064971/143688682-cf30797c-760b-4fc0-aa38-a86e86c6f27f.jpeg)

-  Setting the IP Address Server-ADDS and pointing the DNS to the static IP address used.

![WhatsApp Image 2021-11-27 at 11 02 48 PM](https://user-images.githubusercontent.com/93064971/143688756-b1681206-d960-4559-8ea6-cb8a4b321ee0.jpeg)

-  Click `Promote this server to a domain controller` for ADD configuration
-  
![WhatsApp Image 2021-11-27 at 11 02 49 PM](https://user-images.githubusercontent.com/93064971/143688770-cafd7508-6a1b-498c-85c9-a00518ebd3bf.jpeg)

-  Select `Add a new forest` and enter the domain name to be used in the Root Domain Name. For example here I use the domain `rifqi.com`

![WhatsApp Image 2021-11-27 at 11 02 51 PM](https://user-images.githubusercontent.com/93064971/143688782-001e743f-ab83-4a9b-8919-fcdbbf00edb5.jpeg)

-  Select `Windows Server 2016` at the functional level, put a check mark on `Domain Name System (DNS) server` and `Global Catalog (GC)`. 
   And fill in the Directory Services Restore Mode password with strong password criteria.

![WhatsApp Image 2021-11-27 at 11 02 52 PM](https://user-images.githubusercontent.com/93064971/143688787-572dffe9-0955-4d31-955d-9a18e33f0128.jpeg)

-  then click `Next`

![WhatsApp Image 2021-11-27 at 11 02 52 PM (1)](https://user-images.githubusercontent.com/93064971/143688795-e545c37f-850c-404c-9cee-717a2690e7a1.jpeg)

-  Fill in `The NetBIOS domain name` according to the domain name used.

![WhatsApp Image 2021-11-27 at 11 02 52 PM (2)](https://user-images.githubusercontent.com/93064971/143688803-af4a9f4a-ecf4-4894-b136-3184a2da40aa.jpeg)

-  Skip the Paths section, click `Next`.

![WhatsApp Image 2021-11-27 at 11 02 56 PM](https://user-images.githubusercontent.com/93064971/143688844-ceeb0ace-5bc8-4aa0-a958-6083081669ef.jpeg)

-  Check the configuration specified in `Review Options`, if it is TRUE. Click `Next`.

![WhatsApp Image 2021-11-27 at 11 02 58 PM](https://user-images.githubusercontent.com/93064971/143688857-c7a92ecb-feee-4b0b-ad9d-e4aa455503b1.jpeg)

-  If there is `All prerequisite checks passed successfully.` Click `Install` to apply the specified configuration.

![WhatsApp Image 2021-11-27 at 11 02 58 PM (1)](https://user-images.githubusercontent.com/93064971/143688860-7678f5ff-dd75-4238-aa4e-1cdb788bd34e.jpeg)

![WhatsApp Image 2021-11-27 at 11 02 58 PM (2)](https://user-images.githubusercontent.com/93064971/143688875-66104205-9d43-437a-ad49-39d20b3862a3.jpeg)

-  After the installation is complete, the laptop will restart automatically. Then login using administrator password

![WhatsApp Image 2021-11-27 at 11 02 59 PM](https://user-images.githubusercontent.com/93064971/143688877-4ea8e985-094f-46e5-933d-66a7c4f6a30e.jpeg)

-  To check the configuration results, open `cmd` and type `netdom query fsmo` or check server manager if it green it's all good

![WhatsApp Image 2021-11-27 at 11 02 59 PM (1)](https://user-images.githubusercontent.com/93064971/143688891-ea1a2a05-774b-45ea-a0d6-27bf0ccbc831.jpeg)

![WhatsApp Image 2021-11-27 at 11 02 59 PM (2)](https://user-images.githubusercontent.com/93064971/143688924-0ec0a8a3-5779-4e37-b468-b2d89e2bde0d.jpeg)

-  DONE .*^_^*.  
