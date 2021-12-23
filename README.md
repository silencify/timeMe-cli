# timeMe-cli

## Setup
1. Add following environment variables in `.bashrc`
    ```
        export WORKSPACEID=''
        export PROJECTID=''
        export USERID=''
        export APIKEY=''
    ```
2. Run command `source ~/.bashrc`
3. Update `CURRENTDATE` on basis of timezone. Takes time in UTC.
4. Run command `chmod +x clockify`
5. Move `clockify` file to `/usr/local/bin`

The clockify can be used as command on terminal. See below for usage

## Usage
1. `clockify start standup` - starts standup task.
    - Edit message on the `clockify` file for custom message.

2. `clockify start new "$task"` - starts new task.
    - It creates the task
    - Assignes the task to yourself
    - Start the timer.
    - eg. `clockify start new "TASK-001"`

3. `clockify start $task` - starts already created task.
    - eg. `clockify start TASK-001`

4. `clockify stop` - stops the current running timer.
