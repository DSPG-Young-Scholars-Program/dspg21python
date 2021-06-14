# **Setting up Python Environments in Rivanna**

![](RackMultipart20210614-4-1v0mrl0_html_66621ba9c1ea09b5.gif)

# **May 2021**

This is documentation on how to set up the virtual environment recommended for working with Python inside Rivanna. This document was created in September 2020 and last updated on May 2020. This is specific to Rivanna, and was originally authored by Martha Czernuszenko ([mc9bn@virginia.edu](mailto:mc9bn@virginia.edu)), DSPG2020 Fellow. You can direct any questions to Neil Kattampallil ([nak3t@virginia.edu](mailto:nak3t@virginia.edu))

**Part 1: Setting up a virtual conda environment on**

**Rivanna**

**Step 1.1: Open Cluster**

a. Open Rivanna Shell Access from Clusters

![](RackMultipart20210614-4-1v0mrl0_html_5cb2ec127e8a1c2d.gif)

**Step 1.2: Activate conda**

a. Enter _module load anaconda/5.2.0-py3.6_

b. Enter _conda env list_ (this is a check and sees which conda environments you have)

![](RackMultipart20210614-4-1v0mrl0_html_ff71f423fd4704c4.gif)

**Step 1.3: Create Virtual Conda Environment by entering:** (do not add a space in your name)

a. Enter _conda create --clone pytorch-0.2.0-py3 --name &quot;Your environment name here&quot;_

Example: **conda create --clone pytorch-0.2.0-py3 --name &quot;martha\_bert&quot;**

\*This process will take a while, probably 5-10 minutes

![](RackMultipart20210614-4-1v0mrl0_html_ee95574c419e73c1.gif)

**Step 1.4:**

a. Activate Virtual Environment: Enter _source activate &quot;environmentname&quot;_

Example: source activate &quot;martha&quot;

![](RackMultipart20210614-4-1v0mrl0_html_feeb71f981c42140.gif)

**Step 1.5: Check if your virtual environment has been created:**

a. Enter _conda env list_

(should be in your user id folder)

![](RackMultipart20210614-4-1v0mrl0_html_a0fda59723a08c97.gif)

**Step 1.6: Install to switch conda environment via kernel:**

**a.** Enter _conda install nb\_conda_

**Step 1.7:** Exit Rivanna Shell Access.

**Part 2:**

**Step 2.1: Launching a Rivanna Session**

(You have to launch a new session or your environment won&#39;t show)

1. Rivanna Partition: BII-GPU

2. Optional: GPI type for GPU partition: NVIDIA P100

![](RackMultipart20210614-4-1v0mrl0_html_8c1bb41cd2b957d8.gif)

**Step 2.2: Start a new Jupyter Notebook (File \&gt; New \&gt; Notebook)**

A. Rivanna should prompt you on this message:

![](RackMultipart20210614-4-1v0mrl0_html_8e9234158ac74017.gif)

B. Select your environment.

a. If you don&#39;t see your environment here, you need to go back to shell access and take these steps:

i. _module load anaconda/5.2.0-py3.6_

ii. _conda env list_

Do you see your environment?

a. Yes! (This means your environment was created, but you need to enter _conda install nb\_conda_ to see your environment

b. No? Go back to step 1.1

![](RackMultipart20210614-4-1v0mrl0_html_4fc6b8278e89e8b7.gif)
