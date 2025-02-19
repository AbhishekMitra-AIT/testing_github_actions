# testing_github_actions

1. Enable branch protection rules in your repository settings:

    ```markdown
    Go to Settings > Branches
    Add a branch protection rule for your main branch
    Check "Require status checks to pass before merging"
    Select this line length check as a required status check
    ```

2. Inside Target branches > Branch targeting criteria > add target(include default branch and include all branches)

3. Inside Actions > New Workflow > setup a workflow yourself > add the details of yml file and give a name to yml file with its extention.

4. Inside test1.py uncomment the 160 char lines and push the code. The test will fail. Again comment the 169 char lines and uncomment the lines less than 160 char, push the code and check if the test passes.

This will prevent any code from being merged if it contains lines longer than 160 characters.