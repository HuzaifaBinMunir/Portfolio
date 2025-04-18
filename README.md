# Portfolio
This is my portfolio website

## Step 1: Project Initialization & Basic Setup
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

Navigate into your newly created project folder. Run:

**cd my-portfolio**

Step 2: Run npm install again inside your project

**npm install**

While it is being downloaded you will be asked the following questions: 

![image](https://github.com/user-attachments/assets/9a441136-d432-4211-ace7-fdcecc76d65c)

Here's what each selection means:

**1) TypeScript:** Choose Yes (default JavaScript, simpler if you’re unfamiliar with TypeScript).

**2) ESLint:** Choose Yes (helps maintain code quality).

**3) Tailwind CSS:** Choose Yes (recommended styling framework).

**4) src/ directory:** Choose Yes (organized file structure, recommended).

**5) App Router:** Choose Yes (modern Next.js routing, recommended).

**6) Turbopack:** Choose Yes (faster builds and better performance).

**7) Customize import alias:** Choose Yes (custom shortcut paths for cleaner imports).








