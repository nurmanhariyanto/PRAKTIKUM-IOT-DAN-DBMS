# PRAKTIKUM IOT DAN DBMS
MENGGUNAKAN .NET CORE SDK DAN RUNTIME   
**Tutorial ini menggunaan Windows 10/11**

Tools / Hardware yang digunakan: 
- Komputer/PC/Laptop dengan OS Windows 10/11
- Mouse
- Keyboard
- Kabel HDMI 
- Monitor

1. Download dan install dotnet sdk pada proses ini **Memerlukan koneksi internet dan pada tutorial ini menggunakan versi .NET 8.0 LTS**
    - Link download sdk -> https://dotnet.microsoft.com/en-us/download
    - Untuk Instalasi sdk -> https://learn.microsoft.com/en-us/dotnet/core/install/windows?tabs=net80
    - Tutorial ini menggunakan visual studio code sebagai code editor yang dapat di download di -> https://code.visualstudio.com
      
    
         
2. Menambahkan nuget package pada project di Visual studio code
      Untuk menambahkan nuget package harus menginstall plugin https://marketplace.visualstudio.com/items?itemName=NuGetTeam.NuGetPackageManager
      Jika sudah berhasil di install reload visual studio code
      
      setelah itu tekan *Ctrl+shift+P* makan akan muncul dialog pilih *Nuget Package Manager: Add Package*
      Masukan nama package yang akan di install
      Pilih versi package
      
      Setelah itu gunakan perintah berikut untuk rebuild project
      ```
      dotnet restore
      dotnet run
      ```

2. Instalasi rabbitmq server dapat mengikuti tutorial berikut : https://www.linkedin.com/pulse/how-install-rabbitmq-windows-gitonga-bretton/
   aktifkan plugin mqtt pada rabbitmq dengan cara masuk ke directory rabbitmq C:\Program Files\RabbitMQ Server\rabbitmq_server-xxxxxx\sbin
   plugin management
   ![alt text]([http://url/to/img.png](https://media.licdn.com/dms/image/D4D12AQH99RpRDtvowQ/article-inline_image-shrink_1500_2232/0/1695803035859?e=1709769600&v=beta&t=upbGDpqBtXiwxRHrKJ0P_OiETPlwFirGK_bC2nHZxR0))
   
    ```
      .\rabbitmq-plugins.bat enable rabbitmq_management
      ```
   plugin mqtt
   
     ```
      rabbitmq-plugins enable rabbitmq_mqtt
      ```
         
         
# [**Contoh Program**](https://github.com/nurmanhariyanto/absensi-iot)

         
          
