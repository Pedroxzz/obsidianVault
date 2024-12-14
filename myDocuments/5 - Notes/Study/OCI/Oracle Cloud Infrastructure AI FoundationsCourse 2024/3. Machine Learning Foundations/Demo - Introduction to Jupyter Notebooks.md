---
tags:
  - oci
Index: "[[3. Machine Learning Foundations]]"
---
# Transcript 
Hello, and welcome again to our course on OCI Foundations. Before we start with a machine learning use case, we will first talk about a powerful tool that's a must have in the toolbox of any aspiring data scientist.

What is Anaconda? So Anaconda is an open source distribution of Python and R for data science and machine learning. It's designed to simplify package management and deployment. So think this as a toolbox that comes preloaded with all the essential tools and libraries you will need to kick start your journey into the world of data science and machine learning.

Now, you might be wondering why to use Anaconda? Well, there are several good reasons why Anaconda is one of the most widely used data science tools. First of all is the package management. Anaconda makes it incredibly easy to install and manage data science libraries and packages. Anaconda allows you to create isolated environments for your projects. This means you can work on multiple projects with different package versions without any conflicts.

A third one is this Anaconda Navigator itself, a very user-friendly interface to manage your environments, install packages, and launch Jupyter Notebooks all without needing to use the command line. And again, this is a cross-platform tool, so whether you are using Windows, Mac, or Linux, Anaconda is available for all major operating systems.

The one tool in particular, which we are going to use for our machine learning use case is this Jupyter Notebook. Jupyter Notebook is a powerful, interactive development environment, which we usually call IDE that allows you to create and share documents containing live code equations, visualizations, and narrative text.

This is a very fantastic tool for prototyping data exploration and creating interactive presentations. Let's launch this. And our Jupyter Notebook server is launched in your local machine, and you will see a tab in your browser similar to this here. You can see two tabs here Files and Running. Files will show you all existing files and folders, and Running will show you your existing terminals or notebooks.

Third tab here are Clusters. This is for parallel processing, but again, it's out of scope for this demo. So going back to your Files, let's create a new folder. There is a folder called Untitled just created seconds ago. Click on that and rename it. And we will just call it MLDemo. OK. So we have our folder created. So if you double click on that folder, it says the Notebook list is empty. Let's create a new Notebook.

I have this Python 3 kernel. Click on that. Clicking on that took me to this new tab, which is a Notebook where we will write our codes. First rename this to MLDemo1. one And you can do just by simply clicking on this untitled, and I will name it MLDemo1. click on Rename, and you will see now it renames this Jupyter Notebook. So now let's write a few lines of Python code, and let's see how this cell works actually.

To comment you start with a hash. So I'm going to write #This program adds two numbers, OK. So I will create my first variable num1 = 1, num2 = 4. And I will add another comment, #Add two numbers. And I will write another variable sum, and write num1 + num2. You can either run it from here, or you can also click Shift+Enter on your keyboard. You can also press Shift+Enter on your keyboard, and this will run this cell.

In the next cell, I will display the sum, and I will write a print statement. "The sum of-- let's say-- (0) and (1) is (2)", format, (num1, num2, sum). On running this cell, you can see the result. So this is our very basic Python code. The sum of 1 and 4 is 5. This is how you run any code in your cell. So now we will start with our first demo.