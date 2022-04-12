# Trello Due Today

Simple tool to keep Trello overdue tasks due to date (for people with too many tasks to manage)

## Configure and Run

1. Clone the Repository
2. Run `npm install`
3. Create _.env_ file in root directory with the following structure:

```
API_KEY=
API_TOKEN=
LIST_ID=
BOARD_ID=
```

4. The Api Key and Api Token can be generated at https://trello.com/app-key
5. The Board Id can be obtained from the board url:

![image](https://user-images.githubusercontent.com/37779707/162958849-d18595bf-04f3-447b-a9b7-fbeb71f334a6.png)

6. Populate the previous three fields and run `npx tsc --build`
7. To obtain the List Id run `npm run listid`. The console will show you the board's lists and you can copy the id of the wanted list.
8. To start the program run `npm start`

And you're done!
Every overdue task in the provided list will be updated with a new due date set to the end of today.

## Notes

Some workplaces have a particular SSL protection, the following line on top of both index.ts and listid.ts can be uncommented if you want to bypass that protection:

`// process.env["NODE_TLS_REJECT_UNAUTHORIZED"] = '0';`
