# Reading - API Deployment
## Django Settings: Best Practices
### Managing Django Settings: Issues
* Different Environments
  * There are multiple environments, local, dev, staging ect
  * Each can have their own settings
  * Use an approach that you can keep all of them
* Sensitive Data
  * Use your SECRET_KEY wisely along with DB passwords
* Sharing settings between team members
  * Use a general approach to eliminate human error
 
### Setting Django Configurations
* settings_local.py
  * The oldest method
  * Setting all environment-specific settings in this file which is ignored by VCS
  * Pros:
    * Secrets not in VCS
  * Cons:
    * settings_local.py is not in VCS so you can lose some settings
    * Its python code so there can be non-obvious logic
    * Need settings_local.example to share default configs for devs
* Separate settings file for each environment
  * Pros:
    * All environments are in VCS
    * Easy to share between devs
  * Cons: 
    * Need to find a way to handle secret passwords and tokens
    * "Inheritance" of settings can be hard to trace/maintain
* Environmental Variables
  * Pros:
    * Configuration is separated from code
    * Environment parity - you have the same code for all environments
    * No inheritance in settings and cleaner/more consistent code
    * Theoretical grounding for using environment variables - 12 Factors
  * Cons:
    * You need to handle sharing default config between devs

* 12 Factors
  * Codebase
  * Dependencies
  * Config
  * Backing Services
  * Build, release, run
  * Processes
  * Port Binding
  * Concurrency
  * Disposability
  * Dev/prod parity
  * Logs
  * Admin Processes

### Django-environ
* Writing code with os.environ is like a merge of:
  * envparse
  * honcho
  * dj-database-url
  * dj-search-url
  * dj-config-url
  * django-cache-url

### Django Settings: Best practices
* Keep settings in environmental variables
* Write default values for production config, exclude secret keys and tokens
* Don't hardcode sensitive settings and don't put them in VCS
* Split settings into groups: Django, third-party, project
* Follow naming conventions for custom (project) settings
