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

- Access the menu `Input – Keyboard – Insert Ctrl + Alt + Del`. Enter the password created and wait for the configuration to load

- Windows Server 2022 has been successfully installed

### B. Instalasi Active Directory Domain Services
-  Before doing the installation, we change the computer name first by going to windows powershell.
   Then type `rename-computer -Newname Server2022`
    - Open the start menu and select `Windows PowerShell`
    ![2021-11-27](https://user-images.githubusercontent.com/93064971/143680317-558a5359-fee6-47e3-a71d-e5457e851809.png)
```
Then Restart, and open`Server Manager` 
```
- Select Menu `manage`, Then `Add Rules and Features` 
![2021-11-27 (2)](https://user-images.githubusercontent.com/93064971/143680344-f47e1d37-f2c9-48cd-9f49-2749d820e1ed.png)
![2021-11-27 (1)](https://user-images.githubusercontent.com/93064971/143680443-751e7129-047f-420f-b3e7-9b1e815691be.png)

- Select Next
![2021-11-27 (12)](https://user-images.githubusercontent.com/93064971/143680477-8233204f-6bc9-4e6b-b50a-a76db08c3a7e.png)

- Select option`Role-based or feature-based installation`. And `Next`


- Click `Select a server from the server pool` to select a local storage directory. Then `Next`

- Next, put a check mark in the `Active Directory Domain Services` box. When you check the box, on the right appears 
  a brief description of ADDS and how it works. Then click `Add Features`.
  
### C. Instalasi DNS server

