# Welcome to your new dbt project

This tutorial makes use of **Visual Studio Code (VSC)** as the **IDE**, **Snowflakes** as the **data warehouse**.

I will attempt to be very detailed in my explanations as to using **dbt** with **Snowflakes**

## Creating a snowflakes account

As a new user: simply navigate to the [snowflakes sign up page](https://signup.snowflake.com/?_ga=2.39988834.1303182868.1634285132-1006226680.1634285132) and get started with the 30-days free trial (you can do an actual subscription if you can afford one). Proceed to fill in your details, and an activation mail will be sent to your email. click on the activation link and chose a user name, your preferred cloud provider **(Google Cloud, Microsoft Azure, or Amazon Web Services)**. Thereafter, you can proceed to the login page. (You will want to bookmark this page for easy accessibility)

Now take note of your username, account_link (something like this: **mf.....**.us-central1.gcp) this assumes that I am using gcp as my cloud provider, and my **data center** is in us-central. 

Click on the icon where your username is captured, select switch role (account admin is what is used in this tutorial, you might want to try something else).

You also need want to check for the following:

- warehouse name
- Database name
- Schema

### Initializing dbt Project

To get started:

- Install the dbt module on your computer using "pip command": **"pip install dbt"**. You can verify the information about your current installed version using **"pip show dbt"** command.
- Create an empty folder/directory on your computer.
- Create a new repository on your github account do not select the **.gitignore, README.md and LICENSE** options (optional, but a good practice).
- Copy the link to the repository you have just created.
- From your IDE (VSC), navigate to the folder you created in step 1, and clone the repository into the new directory created using the **"git clone"** command.
- Initialize your dbt project using the **"dbt init"** command. Here, you will need to give your project a name. The command for this is: **"dbt init [project_name]"**
- Once you are done doing this, if you navigate to your **home directory** (for windows users: C:/Users/account_name; for linux users: /home/account_name), you notice that a new folder/directory **(.dbt)** has been created there (you may have to enable the **show hidden files** option on your computer to be able to view this folder). There are two files in this directory; **profiles.yml** and **users.yml**.
- Now open the **profiles.yml** file with your editor, and update the content with appropriate details. A sample template **(profiles.ym)** is attached in this repository.

You will notice from the initialized project that new files and directories are being added to your current directory.

After updating the **profiles.yml** file, navigate back to the **dbt_project.yml** file and change the model name to name of your initialized model. Thereafter, proceed to towards the end of the page, and update the model name to match with the earlier stated name.
  
### Using the starter project

Try running the following commands:

- dbt debug (if this run successfully, then you are ready to start exploring **dbt** leveraging the full power of **snowflakes**)
- dbt seed (to upload the attached csv file in __Data__ folder to your snowflake warehouse)
- dbt run
- dbt test

### Resources

- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices.
- Learn more about snowflakes [in the docs](https://docs.snowflake.com/)

__Author:__ Muhammad Abiodun Sulaiman

__Email:__ prince.behordeun@gmail.com or abiodun.msulaiman@gmail.com

__LinkedIn:__ [Muhammad Abiodun Sulaiman](https://www.linkedin.com/in/muhammad-abiodun-sulaiman)

__Twitter:__ [@Prince_Analyst](https://wwww.twitter.com/Prince_Analyst)

__Facebook:__ [Muhammad Abiodun Sulaiman](https://www.facebook.com/muhammad.herbehordeun)

__Tel:__ +2348108316393

![My Pix.png](https://user-images.githubusercontent.com/45925374/140731559-e56f334c-8e89-48b8-92f7-fbe66a7447d9.png)
