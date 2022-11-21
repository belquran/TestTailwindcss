# TestTailwindcss
//right click on your sln project and select open in terminal

npm install -D tailwindcss cross-env
npx tailwindcss init

npm init -y

//create input.css file and type below code inside it

@tailwind base;
@tailwind components;
@tailwind utilities;



//add below code in .csproj file

 <Target Name="Tailwind" BeforeTargets="Build">
        <Exec Command="npx tailwindcss -i ./wwwroot/css/input.css -o ./wwwroot/css/output.css" />
 </Target>







Link:
https://github.com/Practical-ASP-NET/Tailwind.Extensions.AspNetCore
https://tailwindcss.com/docs/installation