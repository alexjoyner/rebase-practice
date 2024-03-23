# rebase-practice
Just messing around to try and understand rebase better

Key Takeaways:
- Rebase into feature branches to keep git history clean
		!!! MAKE SURE NOONE ELSE USES A BRANCH THAT YOU REBASE! REBASES SHOULD PRIVATE TO THE REBASER
		this is because it will re-write the git history and will fuck with someone else if they have a different history

Process While On Feature Branch to pull updates from the main branch
- Make sure main is up to date
- Checkout feature branch
- git rebase main
- git push origin [FEATURE BRANCH NAME] --force
	- Need to force push to remote because now the remote branch history is out of date with the local version
