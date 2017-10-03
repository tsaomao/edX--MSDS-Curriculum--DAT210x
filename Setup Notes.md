# Notes/Intro
This machine has both Python 2 (installed as python) and Python 3.5-3.6 (installed as python3) on it. So it was necessary to install, run, and configure anaconda and jupyter with environments to make a distinction and run Python 3 for compatibility with this class.

# Setup Deviations
Contrast to Lab setup instructions here:
1. [Installing Anaconda and Python](https://courses.edx.org/courses/course-v1:Microsoft+DAT210x+4T2017/courseware/61640bd8-06eb-fd61-8000-024d0471b794/f6115c15-8327-6aec-be0c-346579082aab/?activate_block_id=block-v1%3AMicrosoft%2BDAT210x%2B4T2017%2Btype%40sequential%2Bblock%40f6115c15-8327-6aec-be0c-346579082aab)
    * For commands using "pip", I used "pip3" instead. So e.g. `sudo pip3 install BeautifulSoup4` instead of `sudo pip install BeautifulSoup4`
2. [Using Jupyter](https://courses.edx.org/courses/course-v1:Microsoft+DAT210x+4T2017/courseware/61640bd8-06eb-fd61-8000-024d0471b794/f6115c15-8327-6aec-be0c-346579082aab/?activate_block_id=block-v1%3AMicrosoft%2BDAT210x%2B4T2017%2Btype%40sequential%2Bblock%40f6115c15-8327-6aec-be0c-346579082aab)
    * In the **Basic Commands** section, before moving forward with the conda and jupyter installs, I first used conda environment management commands to create a virtual environment called "py36" running python 3.6.
    * For that, I ran the command: `conda create -n py36 python=3.6` and then `source activate py36` (See link listed as "Managing environments" in **Additional Resources** below.)
    * It's now important to remember to start any of this work now with `source activate py36` and to stop using the virtual environment when done, with `source deactivate`.
    * Within the *activated* and *correct* virtual environment (py36), the given commands in **Basic Commands** are correct.
        * Note that this environment is now missing key portions of the setup, so be aware that you have to run `sudo pip install ...` commands to redress this when the Jupyter notebook runs - there will be misss module errors.
3. [Using Spyder](https://courses.edx.org/courses/course-v1:Microsoft+DAT210x+4T2017/courseware/61640bd8-06eb-fd61-8000-024d0471b794/f6115c15-8327-6aec-be0c-346579082aab/?activate_block_id=block-v1%3AMicrosoft%2BDAT210x%2B4T2017%2Btype%40sequential%2Bblock%40f6115c15-8327-6aec-be0c-346579082aab)
    * Unable to figure out how to get this to run python3. Partly due to my having a previous install of anaconda that's also confusing things. Will update if it becomes important and I figure it out.
4. Additionally, I created an unlinked/detached GitHub clone/download [repo](https://github.com/tsaomao/edX--MSDS-Curriculum--DAT210x) of the provided [course repo](https://github.com/authman/DAT210x), so I need to remember to maintain my copy with appropriate GitHub pushes to the remote, 'origin', which resides on GitHub, to show my work to the world.

# Additional Resources
In addition to my own experimentation, I also used the following guides, tutorials, and documentation:
* [Installing Jupyter Notebooks](http://jupyter.readthedocs.io/en/latest/install.html) - Not that helpful but a good baseline.
* [Managing environments](https://conda.io/docs/user-guide/tasks/manage-environments.html#removing-an-environment) - About using virtual environments within anaconda so I can use andd specify the version of Python while setting up Jupyter Notebooks with the right version of Python (3.6) for the course.
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - For help writing this.
* [Dual Installations of Python 2.X and Python 3.X with Anaconda/Spyder](http://lifeofajenni.com/2017/02/22/python-2x-and-3x-in-spyder/) - Information was helpful but didn't apply to my situation quite right.
