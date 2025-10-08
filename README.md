
## Bookmarking API Endpoints

### `/bookmarks`
| Endpoint                    | Method | Description                                                    |
| --------------------------- | ------ | -------------------------------------------------------------- |
| `/:username`                | POST   | Add a bookmark for the specified user                          |
| `/:username`                | GET    | Retrieve all bookmarks for the specified user                  |
| `/:username/:questionId`    | DELETE | Delete a specific bookmark by question ID for the specified user |

### `/collections`
| Endpoint                                      | Method | Description                                                    |
| --------------------------------------------- | ------ | -------------------------------------------------------------- |
| `/:username`                                  | POST   | Create a new collection for the specified user                 |
| `/:username`                                  | GET    | Retrieve all collections for the specified user                |
| `/:username/:collectionId`                    | PUT    | Update a collection's name or properties                       |
| `/:username/:collectionId`                    | DELETE | Delete a specific collection                                   |
| `/:username/:collectionId/bookmarks`          | POST   | Add a bookmark to a specific collection                        |
| `/:username/:collectionId/bookmarks/:bookmarkId` | DELETE | Remove a bookmark from a specific collection                   |
| `/:username/:collectionId`                    | GET    | Get all bookmarks within a specific collection                 |
