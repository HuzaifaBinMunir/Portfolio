# Portfolio
This is my portfolio website

## Ticket 1: Project Initialization & Basic Setup
-> Install Next.js

Run the following commands: 

**1) npx create-next-app@latest my-portfolio** 

**2) cd my-portfolio**

### Error1:

I got the following error 
![image](https://github.com/user-attachments/assets/e024d84f-e2c5-405b-a408-a9e5fb1bff0e)

#### How to quickly fix this issue:
Step 1: Create the missing npm directory using the following command

**mkdir C:\Users\huzai\AppData\Roaming\npm**

Step 2: Clear npm cache

**npm cache clean --force**

Step 3: Verify 

**npm -v**

**npm install**

### Error2:

I got the following error:
![image](https://github.com/user-attachments/assets/abda3de2-ec89-4c3b-a966-8b2d978b5252)

#### How to Fix this Error:
Step 1: Navigate to your project directory if already created otherwise run: 

**npx create-next-app@latest my-portfolio**

While it is being downloaded you will be asked the following questions: 

![image](https://github.com/user-attachments/assets/9a441136-d432-4211-ace7-fdcecc76d65c)

Here's what each selection means:

**1) TypeScript:** Choose Yes (default JavaScript, simpler if you’re unfamiliar with TypeScript).

**2) ESLint:** Choose Yes (helps maintain code quality).

**3) Tailwind CSS:** Choose Yes (recommended styling framework).

**4) src/ directory:** Choose Yes (organized file structure, recommended).

**5) App Router:** Choose Yes (modern Next.js routing, recommended).

**6) Turbopack:** Choose Yes (faster builds and better performance).

**7) Customize import alias:** Write @/* (custom shortcut paths for cleaner imports).

![image](https://github.com/user-attachments/assets/daa91455-369b-47bb-9045-1985b1e69cd4)

Navigate into your newly created project folder. Run:

**cd my-portfolio**

Step 2: Run npm install again inside your project

**npm install**

![image](https://github.com/user-attachments/assets/f2684c93-a030-4718-8e56-23e2957732ca)


Step 3: Run:

**npm run dev**

![image](https://github.com/user-attachments/assets/6228b561-bc26-4168-a865-760a8d8c5fe5)

![image](https://github.com/user-attachments/assets/68f11eda-4530-4300-a5aa-f6c640a09d17)

**NOTE**: If you want to terminate it press Ctrl + C in your terminal to stop the Next.js dev server.

Now it is running successfully. 

Go to **http://localhost:3000/** to verify. 

![image](https://github.com/user-attachments/assets/0935e3c7-8114-478d-8163-403456b032f8)

I think it is 100% good now!
The fact that I see this screen means:

1) Next.js is running perfectly.
2) My development server is live at http://localhost:3000
3) The terminal is supposed to keep running — it's not supposed to "end" like other one-time commands. It keeps running to:

Watch for changes

Auto-reload the browser when you update your code

## Ticket 2: Define Folder Structure & Static Data

-> Step1: Create folders inside src like components, assets and data. Run:

**mkdir -p src/data**

**mkdir -p src/components**

**mkdir -p src/data**

![image](https://github.com/user-attachments/assets/6f355ceb-13c0-4e6b-9f30-543300ba31dd)


->  Step 2: Create projects.ts file with your static data
![image](https://github.com/user-attachments/assets/4cdab61c-31a0-4299-8534-a2fd5893749c)

Made a slight error here. I accidentally created projects.ts as a folder (directory), not a file — that’s why I was't able to open it in VS Code.

NOTE: 
a) I was trying to open the directory manually before to check by the cd command but it didn't work, so now I am using **"cd .."** command to go back to my main directory called my-portfolio.
b) Now, I will remove the previously created erroneous folder by the command: **" rmdir src\data\projects.ts "** 
c) Finally, create the file by using this command: "**New-Item -Path projects.ts -ItemType File"**
![image](https://github.com/user-attachments/assets/7bda28d4-ddc0-4605-b19a-ac59e980e5f1)
d) Write the sample code as shown in my code files. 

## Ticket 3: Build Reusable Components

-> Step 1: Create Header.tsx by the command **"New-Item -Path Header.tsx -ItemType File"**
-> Step 2: Create Footer.tsx by the command **"New-Item -Path Footer.tsx -ItemType File"** 
-> Step 3: Create Layout.tsx by the command **"New-Item -Path Layout.tsx -ItemType File"**
-> Write the sample code as shown in my code files.

![image](https://github.com/user-attachments/assets/57b9ff5c-2ec6-4a45-a980-bec77fad2861)
![image](https://github.com/user-attachments/assets/71994c10-4011-430d-bdf6-2311c46de62e)

->Step 4: Step 4: Use Layout in Homepage
See code files for code to replace in the page.tsc file in src/app/page.tsx

## Ticket 4 — Build the Home and About Pages
->  Step 1: Create the About page with command **" mkdir app/about "**
-> Step 2: Add navigation to your Header.tsx

## Ticket 5 - Projects Page
-> Step 1: Create /projects Page ( In app/ folder Create a new folder called projects, inside that, create a file called ** page.tsx **)

-> Step 2: Build the Basic Projects Page( Copy the code in my file page.tsx) 

-> Step 3: Update Navigation (Add "Projects" Link)

## Ticket 5 - Part2 Projects List

-> Step 1: Create a new component — ProjectCard
Inside your src/components/ folder, create a file::
ProjectCard.tsx

-> Step 2: Paste the code from my file

-> Step 3: Update your projects/page.tsx file

