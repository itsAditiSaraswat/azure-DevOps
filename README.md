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

Once code changes are ready to be integrated into higher level environments, having a build pipeline configured saves a lot of time, and is a reliable way to integrate such changes into your application.

**STEPS**<br>

**Step-1:** Navigate to your Azure DevOps project page by going to dev.azure.com/your-organization-name. On the left-hand navigation menu, find the **Pipelines** option and click on it to go to the pipeline section of your project.
![1](https://user-images.githubusercontent.com/102405945/211164463-563955e1-1665-4b94-bbda-a6fd2da0d218.png)

**Step-2:** To create a new build, click on the **Create pipeline** button in the center of the screen.
![2](https://user-images.githubusercontent.com/102405945/211164467-b7dc8ec7-0eb4-49c1-8ab6-b9c9be7697ba.png)

**Step-3:** You are brought to the build pipeline wizard where it will configure the initial settings for a build. Click the link underneath that says, **"Use the classic editor"**.
![3](https://user-images.githubusercontent.com/102405945/211164472-51f3ae86-f68a-4e00-851b-e7549b2ba446.png)

**Step-4:** Choose the source repository that will be used for this build pipeline. We'll use **Azure Repos Git** for our source. If you already have a repository connected to this project, you'll see that the team project and repository dropdowns are already populated. Click **Continue**.
![4](https://user-images.githubusercontent.com/102405945/211164473-c0315165-97f4-4c7f-9407-9aa09abc0372.png)

**Step-5:**  Now you're given the chance to select from many build templates based on the type of application you are building. Select the **ASP.NET Core (.NET framework)** listed under the other's category, as that's what we're building. Then click **Apply**.
![5](https://user-images.githubusercontent.com/102405945/211164479-fc79757c-6c25-45ef-aea8-4e102b480fad.png)

**Step-6:** Now, click on the arrow and then click the **save** option. A saved build pipeline window will then appear. You can leave the select folder at the root. And if you'd like, you can leave a comment about this build pipeline. Then, just click **Save**.
![6](https://user-images.githubusercontent.com/102405945/211164488-7623fda7-c2ee-41f5-a3d2-675161cc511f.png)

And that's it, you've just created build pipeline for your .NET Core application.



### 3.2 Configure your build steps

Configuring our build means adapting the provided build templates to perform the actual steps we need to build our project. Let's see how to do that with a .NET core build template including the addition of a brand new step.

**STEPS**<br>

**Step-1:** On the left-hand Navigation menu in Azure DevOps project overview, click **pipelines** icon to go to your builds. You should see a list of all your build pipelines and the history of the current one that's selected. Select the build pipeline you'd like to configure.
![1](https://user-images.githubusercontent.com/102405945/211164958-6e035956-6db2-4839-be29-a65624a8ef70.png)

**Step-2:** Towards the top-right of the screen, click on **Edit** button.
![2](https://user-images.githubusercontent.com/102405945/211164960-9399bc01-e41f-4f10-a850-628be7bab059.png)

**Step-3:** You'll be brought to the build's overview page. To add a task, click on the **Plus** button located on the Agent Job One header.
![3](https://user-images.githubusercontent.com/102405945/211164964-ab8ba1a0-dfd7-42c0-a296-4d5a0023b83e.png)

**Step-4:** We will need to add NPM install command to download our front-end dependencies. To quickly search for it, use the search box towards the top-right and enter NPM. The top matching results should display. Click on the task NPM to select it and then add the task by clicking the **Add** button towards the right. 
![4](https://user-images.githubusercontent.com/102405945/211164971-32918649-63c4-4ea4-82c4-de9dd20aa025.png)

**Step-5:** You'll see the NPM task added to the bottom of our phase group. We'll need to move it to the appropriate spot towards the top. To do this, click and drag the right edge of the NPM step to the right position. The last step is to provide the correct path to our package.json file in the working folder that contains package.json field. Make sure to select the parent folder of the package.json file and not the file itself.
![5](https://user-images.githubusercontent.com/102405945/211164974-3d493de1-4127-45a3-8826-8fc8dbd5cc28.png)

**Step-6:** Finally, click on the dropdown menu and click **Save** to save your changes. You can add a comment to describe the changes you have made to this pipeline and then click **Save**.
![7](https://user-images.githubusercontent.com/102405945/211164977-deef9bf6-9fd3-4d20-abf0-8f65a9ad08da.png)

And that's it. Your build is now configured to run the steps outlined in your pipeline.



### 3.3 Add build pipeline triggers

One of the most powerful parts of an automated pipeline is the ability to kickstart processes upon some new code changes being pushed to a repo.

**STEPS**<br>

**Step-1:** Go to the Azure DevOps Project overview page for our project. On the left-hand navigation menu, click on the blue rocket icon to go to your builds. You should see a list of all your build pipelines and the history of the current one that's selected. Select the build pipeline you'd like to set up a build trigger for. Towards the top-right of the screen, you'll click on **Edit** button.
![1](https://user-images.githubusercontent.com/102405945/211165217-c9b814c9-8163-4e07-9c31-12482e7f96d2.png)

**Step-2:** You'll be brought to the builds overview page. Towards the top-left, find the **Triggers** tab and select it. Here, you'll see many trigger options. For now, we'll focus on the continuous integration trigger. In order for build triggers to work, ensure that the Enable Continuous Integration checkbox is selected. When you do, you'll see some more options appear below it. One of those is another checkbox option to batch changes while a build is in progress. This option tries to combine as many changes that belong to the same build into one, including new changes that are pushed to a repo while a build is running. This means you won't have multiple builds running one after the other.
![2](https://user-images.githubusercontent.com/102405945/211165219-266e52bb-3b1c-41f0-8763-e05d3c1b4c4a.png)

**Step-3:** Go to the dropdown and click **Save**. Then click **Save** on the Save Build Pipeline window.
![3](https://user-images.githubusercontent.com/102405945/211165222-c764c219-6474-440f-bd25-ea697767fc52.png)

And that's it. You'll see your build kickoff the next time you push a code change to your remote master branch.



### 3.4 Queue manual builds when necessary
A great part about Azure DevOps is that requeuing builds is an easy process. Let's see how to do that if we ever need to requeue a failed or non-kickstarted build.

**STEPS**<br>

**Step-1:** Go to Azure DevOps project overview. On the left hand navigation menu, find the blue rocket icon and click on it to go to your builds. You should see a list of all your build pipelines and the history of the current one that's selected. Select the build pipeline you'd like to requeue.Towards the top right of the screen, you'll click on **queue** button.
![1](https://user-images.githubusercontent.com/102405945/211165393-4911c397-f655-44c8-bc99-3ffbc5f431bc.png)

**Step-2:** A queue build prompt for your selected build pipeline will appear. This prompt is incredibly helpful if you need to rerun a specific build down to the branch, or tags or commits. For now, we'll leave the agent pool to the default of Hosted VS2017, as that's what our build requires for our .NET core application. Finally, leave the default variables and demands options. Since we are requeuing a previous build, these options don't need to be changed. However, they're there for your use should you need to requeue a very specific build. Lastly, click the Run button towards the bottom right of the prompt.
![2](https://user-images.githubusercontent.com/102405945/211165396-54a7d91a-9080-4dc4-9374-7876e9fe5496.png)

That's it. Your build will be requeued, and start when the next agent is available to run your build.
