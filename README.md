# Polling-SCM-Jenkins

Steps to schedule a freestyle job in Jenkins that polls the SCM every night-

```

1. Create a freesyle build job

2. Add a Git source for repository which has sample Java code for build
Ex- https://github.com/nimblenitin/Freestyle-Jobs-Jenkins.git

3. Add Poll SCM for build triggers.
- In the box that appears, enter the cron syntax to schedule a build every night at 12. (ie) 0 0 * * *

4. Add build step.
- In execute shell add - mvn clean install to build using Maven

5. Test the scheduled build
- After saving the configuration, build and view the console output

```
