# GitHub CoPilot Version Migration Demonstration
** Premise **: Use GitHub CoPilot to facilitate automatic codebase migration from one language version to another

For demonstration purposes, we'll be converting an **Angular 6.1** project to **Angular 19.1**

## Steps

### 1. Acquire migration documentation
Save migration instructions in either an `md`, `txt`, or other similar formats. This can be done via the `curl` command.

Example:
``` bash
curl -s https://angular.dev/update-guide?v=6.1-19.0 > angular-migration-guide.txt 
```

Sample Migration Guide Sources:
- Angular: https://angular.dev/update-guide
- SpringBoot: https://github.com/spring-projects/spring-boot/wiki/Spring-Boot-3.0-Migration-Guide
- NodeJs: https://medium.com/@Games24x7Tech/node-js-v20-upgrade-guide-best-practices-and-performance-insights-f76d7ace09ff

### 2. Identify and create proper directory structure
This can be done via prompts to CoPilot.

Example:
```
Prompt: Generate a comparison between the codebase directories of an Angular 6 and an Angular 19 project
```

### 3. Modify files 
CoPilot cannot operate on files as a batch, you will have to navigate to individual files and prompt CoPilot to make changes

Example:
```
Prompt: @workspace /fix Using #file:angular-migration-guide.txt , conve #file:app.component.ts to an Angular 19 compliant file
```
