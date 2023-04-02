# repository-event-dispatch-action

This action can be used to dispatch an event to the repository that you configure.

This is helpful if you want to trigger an action in repository A by a change in Repository B.

```yaml
 - name: Dispatch Event
        uses: flamestro/repository-event-dispatch-action@v1.1.0
        with:
          token: ${{ secrets.PAT_DISPATCH_EVENT }}
          event: EVENT_NAME
          repository: ${{ secrets.REPO }}
          owner: owner_of_repo_and_username_of_pat
```
