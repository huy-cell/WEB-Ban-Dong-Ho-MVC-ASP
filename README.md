## **Technical Stack**

- **.NET Framework:** 4.5
- **Framework:** ASP.NET MVC
- **API Framework:** ASP.NET Web API
- **Database Language:** SQL Server (T-SQL)
- **ORM:** Entity Framework
- **Data Mapping:** AutoMapper
- **JSON Handling:** Newtonsoft.Json
- **Middleware:** OWIN
- **Pagination:** PagedList.Mvc
- **Email Service:** Send e-Mail using Google Mail (Gmail)
- **UI Template:** AdminLTE
- **Frontend Technologies:** HTML, CSS, JavaScript
- **Libraries:** jQuery, Bootstrap, AJAX, JSON, XML, TinyMCE, autoNumeric, dataTables, Font Awesome, Google Fonts
- **Security:** HTTPS and SSL

## **Tools**

- **Version Control:** Git for Windows
- **Code Repository:** GitHub
- **Code Maintenance:** CodeMaid
- **Collaboration:** Google Drive

## **How to Run Source Code**

1. Download source code
2. Open SSMS: Run `Database\script.sql` to create the database (DB) on localhost.
   - **Authentication Type:** Windows Authentication
   - **DB Name:** WebBanHangMvc
3. Open Visual Studio 2019.
4. Open `WebBanHang.sln`.
5. Open `Web.config`: Change Connection String to point to the DB on localhost.

### **Database for Business Domain**

<connectionStrings>
    <add name="DefaultConnection" connectionString="Data Source=.;Initial Catalog=WebBanHangMvc;Integrated Security=true" providerName="System.Data.SqlClient" />
    <add name="ecommerceEntities" connectionString="metadata=res://*/Models.Ecommerce.csdl|res://*/Models.Ecommerce.ssdl|res://*/Models.Ecommerce.msl;provider=System.Data.SqlClient;provider connection string=&quot;Data Source=.;Initial Catalog=WebBanHangMvc;Integrated Security=true;multipleactiveresultsets=True;application name=EntityFramework&quot;" providerName="System.Data.EntityClient" />
    <add name="testmodel" connectionString="metadata=res://*/Models.Model1.csdl|res://*/Models.Model1.ssdl|res://*/Models.Model1.msl;provider=System.Data.SqlClient;provider connection string=&quot;Data Source=.;Initial Catalog=WebBanHangMvc;Integrated Security=true;multipleactiveresultsets=True;application name=EntityFramework&quot;" providerName="System.Data.EntityClient" />
</connectionStrings>

### **Database for Authentication / Authorization**

<configuration>
    <connectionStrings>
        <add name="DefaultConnection" connectionString="Data Source=.;Initial Catalog=WebBanHangMvc;Integrated Security=true" />
    </connectionStrings>
</configuration>

