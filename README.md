[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15379915&assignment_repo_type=AssignmentRepo)
# Setup
This will download Lab 5 locally, allowing you to work on your scripts and upload (push) them back up to GitHub.

1. Clone your lab repository into your ~/ops445/lab5 directory using SSH:
```bash
git clone <ssh link> ~/ops445/lab5/
```
2. Copy your backed-up work into your new GitHub-linked directory:
```bash
cp ~/old_ops445/lab5/* ~/ops445/lab5/
```

# Submission
1. Run the checking script. Make sure you identify and correct any and all errors in your scripts:
```bash
cd ~/ops445/lab5/
pwd #confirm that you are in the right directory
python3 ./CheckLab5.py -f -v
```
2. Redirect the checking script output into *laboutput.txt*:
```bash
python3 ./CheckLab5.py -v &> ~/ops445/lab5/laboutput.txt
```

3. Commit and push (upload) your lab work:
```bash
git add lab*
git add seneca*
git commit -m "Individual message or note."
git push
```

You can make changes to your scripts and reupload as many times as you like. Make sure you commit+push to do so.

**Note:** Your lab is automatically submitted at the due date and time using the last published code. Any changes you publish after the due date won't be marked or seen by your professor.
