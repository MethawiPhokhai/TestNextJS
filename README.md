Initiate a new React Next.js with Dotnet core project using SPA<br />
<br />
Dotnet itself provided configuration for SPA app using Microsoft.AspNetCore.SpaProxy Package<br />
**Only use version 6.0.11 because the newer version will occur the error**<br />
<br />
<b>How to Setup</b><br />
1. Create a DotNet React web application<br />
2. Replace ClientApp with Next.js ClientApp<br />
3. Config the SPA on .proj file<br />
   3.1 Set SpaProxyLaunchCommand to run npm run dev to start React Next.js in localhost:3000<br />
   3.2 Set SpaProxyServerUrl to localhost:3000<br />
   3.3 Set SpaRoot to indicate the React Next.js ClientApp<br />
<br />
<br />
<b>In the Main function need to setup</b><br />
1. app.UseStaticFiles(); for using static file<br />
2. app.MapFallbackToFile("index.html"); default page when start and not found any pages<br />
<br />
<br />

<b>Detail in this link</b>
<br />
Create an ASP.NET Core app with React in Visual Studio<br />
https://learn.microsoft.com/en-us/visualstudio/javascript/tutorial-asp-net-core-with-react?view=vs-2022
<br />
Overview of Single Page Applications (SPA) in ASP.NET Core<br />
https://learn.microsoft.com/en-us/aspnet/core/client-side/spa/intro?view=aspnetcore-7.0
