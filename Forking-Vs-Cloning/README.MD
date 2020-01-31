# Forking vs Cloning

## Clone
A clone is copy of a git repository. It can be located on a local development workstation, on a fileserver, or in the cloud.
A clone is established with the `git clone` command and keeps a linkage with the repository from which it was cloned, which is called the remote. 
 The linkage allows developers to stay up -to-date with development happening on the remote. Branches can be pushed to or pulled from with `git push` and `git pull`.
 
 ## Fork
 A fork is a special type of clone that is remains hosted. In the same way dev branches insulate  master from new, experimental, or unvetted code, so too do forks. 
 The idea of a fork doesn't exist in git. It is an extra layer of indirection provided by a hosted solution like GitHub or BitBucket. Forks make use of pull requests, which are another feature of a hosted solution. Pull requests declare the intent of the incoming party to merge with a mainline branch. In response, other devs have the chance to comment on the work, and approve or reject the PR.
  
   
 
