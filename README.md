# Trello Due Today
Simple tool to keep Trello overdue tasks due to date (for people with too many tasks to manage)

## Configure and Run

1. Clone the Repository

2. Create .env file in root directory with the following structure:
```
API_KEY=
API_TOKEN=
LIST_ID=
BOARD_ID=
```

3. The Api Key and Api Token can be generated at https://trello.com/app-key
4. The Board Id can be obtained from the board url:

![image](https://user-images.githubusercontent.com/37779707/162939045-a6aeb28b-abc9-4ff2-9139-dabc98108fce.png)

5. To Obtain the List Id populate the previous 3 fields and run `npm run listid`. The console will show you the board's lists and you can copy the id of the wanted list.
6. Run `npx tsc --build`
7. Run `npm start`

And you're done!
Every overdue task in the provided list will be updated with a new due date set to the end of today.
