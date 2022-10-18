# repository-event-dispatch-action

This action can be used to dispatch an event to the repository that you configure.

This is helpful if you want to trigger an action in repository A by a change in Repository B.

```
 - name: Dispatch Event
        uses: flamestro/repository-event-dispatch-action@v1.0.1
        with:
          token: ${{ secrets.PAT_DISPATCH_SERVER_DEPLOYMENT }}
          event: TRIGGER_DEPLOYMENT
          repository: ${{ secrets.DEPLOYMENT_REPO }}
          owner: flamestro
```
