# Azure-DevOps

---
## 1. Create a Web App with the Azure Service

### 1.1 Create a web app in the Azure portal

One of the benefits of working with Azure is it provides a vast library of pre-built resources. We'll use one of the pre-built packages to create a Web App in the Azure portal.

**STEPS** <br>
**Step-1:** Click on **Create a resource**.
![1](https://user-images.githubusercontent.com/102405945/211143422-86d49133-b82f-4ea4-9aa6-dfaaa3f03be0.png)

**Step-2:** Click on **Web App** under Popular Azure Services section.
![2](https://user-images.githubusercontent.com/102405945/211143707-01cc9d80-291b-4fd0-81ba-daf18532056e.png)

**Step-3:** Create a new resource group by clicking **Create new**.
![3](https://user-images.githubusercontent.com/102405945/211143714-0d9f6062-d6b4-4169-93f9-a073298dd488.png)

**Step-4:** For the Publish mode select **Code**, if it isn't already.
![4](https://user-images.githubusercontent.com/102405945/211143716-4ed63063-2409-4ac0-a5dd-6cea8a59de11.png)

**Step-5:** Select **.NET 7 (STS)** option in Runtime stack. Select **Windows** option in Operating System.
![5](https://user-images.githubusercontent.com/102405945/211143719-682a70be-b3ef-41a0-a7f3-4506d3211e5b.png)

**Step-6:** Click on **Create** to create a Web App.
![6](https://user-images.githubusercontent.com/102405945/211143720-1f9b26f8-0570-45bf-b267-6abda4e8008a.png)

Hence, the web app is created.
![7](https://user-images.githubusercontent.com/102405945/211143723-a535d745-c2bd-489f-afcf-c2b32391a059.png)

**Step-7:** Click on **App Services** in the left navigation bar.
![8](https://user-images.githubusercontent.com/102405945/211143735-7b9e0c9d-cd59-4705-8045-e6f95e094be3.png)

**Step-8:** Click on the created app.
![9](https://user-images.githubusercontent.com/102405945/211143748-402278b3-3850-4dbf-8f82-bba8870fffa8.png)

You'll be brought to the Overview page for your App Service. Click on the **Browse** button to the left of the search field. You should see your App Service is up and running template page from Azure.
![10](https://user-images.githubusercontent.com/102405945/211143752-1a1cd180-a69d-47a7-a557-b48ed68a0a43.png)



### 1.2 Create a web app in Visual Studio

One common way to begin developing applications is by creating one through Visual Studio.

**STEPS** <br>
**Step-1:** Click on the **Create a new project** button under the Get Started section.
![1](https://user-images.githubusercontent.com/102405945/211159876-abc58e49-a1d3-48cf-be0b-15098ef3d8dc.png)

**Step-2:** This brings up the selection window where you can search for templates of many popular project types. Select the **ASP.NET Core Web App** Template, then click **Next**.
![2](https://user-images.githubusercontent.com/102405945/211159889-cb33af05-af15-4c6e-80f4-54c222a1b08c.png)

**Step-3:** You're prompted to fill in some basic details about your app like the project name and your save location. Fill out these details as they make sense for your setup. Since we are creating a single project within the solution, also ensure that the place solution and project in the same directory check box is checked. Then, click **Next**.
![3](https://user-images.githubusercontent.com/102405945/211159891-9af62ceb-d48c-419c-b0aa-ce3869c5d849.png)

**Step-4:** The final screen in this wizard asks you to select the type of application you want to create. Find the web app application type and select it. Then click **Create**.
![4](https://user-images.githubusercontent.com/102405945/211159896-e535db5e-1383-4603-b4d7-dc7ded69fa23.png)

After a short wait, your app is created. And that's how to create your web app in Visual Studio.
![5](https://user-images.githubusercontent.com/102405945/211159903-39c12e07-9b1d-4c2a-9de2-f4185a7184a6.png)



### 1.3 Publish your app to Azure

Publishing your application to an Azure App Service allows others to access and engage with it.

**STEPS** <br>
**Step-1:** On the right hand side, look for the solution explorer and right click on the name of your project. From there, a context menu opens. Select the **Publish** option in the menu. If you previous published an app you may already have some configured publishing profiles.
![1](https://user-images.githubusercontent.com/102405945/211159960-e44d75e0-3b7e-41e6-9e56-659e674c2ddd.png)

**Step-2:** Select **Azure** in the Target option.
![2](https://user-images.githubusercontent.com/102405945/211159970-752879e7-cc32-49cd-95dd-64d8b8d7fc9b.png)

**Step-3:** Select **Azure App Service(Windows)** in the Specific target.
![3](https://user-images.githubusercontent.com/102405945/211159977-f912a17e-c26f-4914-a619-0e18d8c347ec.png)

**Step-4:** Fill the fields of subscription name, view and search in the App Service option. If you're signed in to your Azure account, you'll have most of the options prepopulated.
![4](https://user-images.githubusercontent.com/102405945/211159999-6e4c2324-4b3f-4a7e-a9d8-2e2879e5e926.png)

**Step-5:** After confirming these details, click **Create**.
![5](https://user-images.githubusercontent.com/102405945/211160003-f8573f1a-7085-408c-be0f-d7991aa58c84.png)

That's it, Visual Studio deploys your app to the newly created Azure App Service.
![6](https://user-images.githubusercontent.com/102405945/211160007-1435c904-a167-4e20-81a9-236acd944d81.png)


---
## 2. Set Up Source Control for Your App

### 2.1 Initialize a new repo using Azure DevOps

Most applications go through several iterations, either with bug fixes or new feature editions. To keep track of all these changes and to properly version your app, let's set up a new repo using Azure DevOps.

**STEPS** <br>
**Step-1:** In the main search field of your Azure portal located towards the top center of the screen, search for Azure DevOps. Select the **Azure DevOps organizations** search result under Services.
![1](https://user-images.githubusercontent.com/102405945/211160739-44565764-a64f-49a9-b970-ad7c6ad4d722.png)

**Step-2:** This will take you to the Azure DevOps overview. Find the link, **My Azure DevOps Organizations**, towards the bottom left and click on it.
![2](https://user-images.githubusercontent.com/102405945/211160746-4160ea20-9cdd-4fd4-8341-cba814c25570.png)

**Step-3:** This will open a new page that shows your connected organizations.
![3](https://user-images.githubusercontent.com/102405945/211160752-c94d9993-a4cc-4d8c-a537-d3dd2b69f60a.png)

**Step-4:** Before we can create a repo, we'll need to first create an organization. Since you don't have any organizations yet, click on **Create new organization** button.
![4](https://user-images.githubusercontent.com/102405945/211160757-262b64d9-d5b2-475d-b10e-4f6b42220fc3.png)

**Step-5:** You'll start the Azure DevOps organization wizard. Click **Continue** to agree to the terms of service, privacy statement and code of conduct.
![5](https://user-images.githubusercontent.com/102405945/211160765-ad802d0f-0d9a-4418-82d3-bf8e2b2c48b4.png)

**Step-6:** Give your organization a unique name and then click **Continue**.
![6](https://user-images.githubusercontent.com/102405945/211160772-981b50bc-d0e3-4311-a8de-f17530a8ee3f.png)

**Step-7:** Now we'll create our first project within our organization. A project is the top-level container that can hold one or more repos. Click **Create project**.
![7](https://user-images.githubusercontent.com/102405945/211160775-7dcd332b-22ad-4043-8f86-54292907c637.png)

**Step-8:** Click on **Repos** on the right navigation menu.
![8](https://user-images.githubusercontent.com/102405945/211160781-e0d20fd5-d60f-41fc-bd7e-d7e2c7967f89.png)

**Step-9:** Once you're in the repos section, find the **plus** button next to your project name. This should be towards the left hand navigation menu. Click on the plus button. A selection menu will appear, prompting you to select a new item to create. Click on **New repository**.
![9](https://user-images.githubusercontent.com/102405945/211160789-95278bde-0806-4096-816d-b203b38ddcdd.png)

**Step-10:** This will bring you to a "Create new repository" window. Be sure that the type selected is Git as that's the version control system we are using. In the repository name field, enter a name for your Git repo.
![10](https://user-images.githubusercontent.com/102405945/211160793-47665080-b63b-48c0-b331-900894cb2d84.png)

That's it. Your new repo is now initialized and you'll be brought to the overview of your files, which include the fresh README and the gitignore files that we just set up.
![11](https://user-images.githubusercontent.com/102405945/211160797-d57ba6f9-dc7b-42c2-a58a-8a58bd3fc532.png)



### 2.2 Initialize a new repo using GitHub

GitHub is a popular web-based hosting service developers use for their source code management. Let's set up a new repo in GitHub.

**STEPS**<br>

**Step-1:** Navigate to github.com and log in to your account. You are brought to your dashboard. Next to your profile photo or on the left hand side, click on the **Create a repository** link. The Create a new repository page comes up. Here, you'll be asked to fill out a few details about your new repo.
![1](https://user-images.githubusercontent.com/102405945/211161155-d8ea7348-6419-49a6-87ac-5140e1248df1.png)

**Step-2:** First, give your repo a name. Next, fill in a quick sentence or two about your application in the Description field. Though optional, a well-configured repo usually contains a meaningful description. Next, check the Initialize this repository with a README checkbox.
![2](https://user-images.githubusercontent.com/102405945/211161172-6f8daa0d-9fb8-445b-b057-6bb934780849.png)

**Step-3:** Finally, click Create repository.
![3](https://user-images.githubusercontent.com/102405945/211161175-f4ee691d-ba2e-4480-b0f1-3e121cfc0c48.png)

That's it! Your new repo is now initialized and you'll be brought to the overview of your files. It also includes the fresh README and gitignore files we just set up.
![4](https://user-images.githubusercontent.com/102405945/211161179-2c20085d-34e4-40e7-9273-d8a17f0a1995.png)



### 2.3 Set up an existing app on Azure DevOps

If you have a legacy app or existing application that needs to be properly versioned, then connecting an existing app to a repository will let you start keeping track of your apps iterations.

**STEPS**<br>

**Step-1:** In visual Studio, open your application.
![1](https://user-images.githubusercontent.com/102405945/211161419-2e19c702-55ce-4c60-be4d-12e3981fff0d.png)

**Step-2:** Click on the **File** menu, and then click **Add to Source Control**. Visual Studio will now create a local repository for your application.
![2](https://user-images.githubusercontent.com/102405945/211161428-0bd56f3f-b4f4-4def-9207-a08487353771.png)

**Step-3:** Click on **Create and push** button.
![3](https://user-images.githubusercontent.com/102405945/211161436-243463be-aa3f-45f6-8705-a72365994301.png)

That's it. You just created a repo for your existing app and connected it to source control.
![5](https://user-images.githubusercontent.com/102405945/211161448-7ddec568-6e77-4177-a884-c0b78f7270aa.png)



### 2.4 Set up an existing app on GitHub

If you have an existing app that you'd like to start managing in GitHub, then you can use few commands to set up a GitHub repo for your existing application.

**STEPS**<br>

**Step-1:** First, we need to create a new repository on GitHub without the readme or gitignore files. Navigate to github.com and log in to your account. Next to your profile photo, click the **plus** button towards the top right, and then click **New repository**. The Create a new repository page comes up.
![1](https://user-images.githubusercontent.com/102405945/211162045-8e4ea358-dddb-4475-8886-e0979029a30f.png)

**Step-2:** Use the same name for your repo as the existing application that you're trying to connect.
![2](https://user-images.githubusercontent.com/102405945/211162055-aa42e8bd-d6b9-480a-814e-6fe631111836.png)

**Step-3:** Finally, click **Create repository**.
![3](https://user-images.githubusercontent.com/102405945/211162061-0d6ebc87-e4cd-4575-803d-821be1cbf5cf.png)

**Step-4:** Your new repo is now initialized, but before we leave, make sure to copy this link right here, we'll need it later when we have to push our local repository to this new remote that we've just created.
![4](https://user-images.githubusercontent.com/102405945/211162067-53c3a213-7b66-45d4-8182-96925fbf26ac.png)

**Step-5:** Now, open the terminal of your choice and navigate to your existing application's home directory using the cd command. Once there, initialize a new local Git repository by using the **git init** command, then press Enter. You'll see we now initialized an empty Git repository on our local machine. To connect to our local repository, we first need to add a reference to the new remote repository we just created using command **git remote add origin https://github.com/itsAditiSaraswat/another-Coffee-critique.git** command. Type **git add .** to add all of your existing application's files to your local repository, and stage them to be committed. 
![6](https://user-images.githubusercontent.com/102405945/211162071-d137d043-ad0e-4f66-a07a-15810f2499cf.png)

**Step-6:** Then, add a commit message to denote your initial setup by typing **git commit -m**, followed by the commit message in quotes. Since this is our first commit setting up our existing application, we will do "Initial commit, setting up version control for old application", then press Enter.
![7](https://user-images.githubusercontent.com/102405945/211162096-e5440cbc-72e5-449c-96f4-6ed6f41011da.png)

**Step-7:** Type the command **git push -u origin master**.
![8](https://user-images.githubusercontent.com/102405945/211162101-38d4e3aa-4582-4121-9505-38b800994d8e.png)

That's it, your existing application now has a local repository and is connected to your newly created remote repository in GitHub. Now, anytime a change is made on your local repository, or a team member merges some changes into the remote repository, you have an easy way to track and integrate these changes both ways.
![9](https://user-images.githubusercontent.com/102405945/211162105-345aa069-d56b-4e02-ae89-75d591413f8f.png)



---
## 3. Configure a Continuous Integration Pipeline

### 3.1 Create a build pipeline in Azure DevOps

**STEPS**<br>

**Step-1:**
