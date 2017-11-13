git diff --name-status commit1 commit2 | awk '{ if ($1 != "D") print $2 }' | xargs git archive -o output.zip HEAD
