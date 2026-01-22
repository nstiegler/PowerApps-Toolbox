# Comment Log

A reusable Canvas Component for displaying and adding comments with user attribution and timestamps.

## Preview

A scrollable comment history panel with a text input and send button at the bottom. Comments display username, timestamp, and message in styled cards. Shows "No comments listed" when empty.

## Tags

`ui` `form` `component` `comments` `collaboration`

## Required Variables

This is a **Canvas Component** (not a simple control). It uses internal collections and custom properties.

| Property | Type | Purpose |
|----------|------|---------|
| `SelectedRecord` | Record | Input: Record containing existing comments as JSON string in `.Comments` field |
| `Props` | Record | Input: Configuration for visibility and placeholder text |
| `State` | Record | Output: Current component state including comment gallery items and new comment input value |
| `OnSaveButtonClick` | Action | Triggered when save button is clicked |
| `OnSendButtonClick` | Event | Custom event fired after comment is saved |

## Setup

1. Import this as a **Component** in Power Apps Studio (not a screen control)

2. Add the component to your screen

3. Configure the `SelectedRecord` property to pass existing comments:
   ```
   SelectedRecord: {Comments: YourDataSource.CommentsField}
   ```

4. Handle the `OnSendButtonClick` event to persist comments:
   ```
   OnSendButtonClick: Patch(YourDataSource, YourRecord, {Comments: JSON(Self.State.CommentGallery.Items)})
   ```

## Data Format

Comments are stored as JSON with this structure:
```json
[
  {
    "Date": "1/22/2025",
    "CommentDate": "2025-01-22T10:30:00",
    "User": {
      "Name": "John Doe",
      "Email": "john@example.com"
    },
    "Comment": "This is a comment"
  }
]
```

## Customization

- **Width:** Modify `Width` property on the component (default: 350)
- **Height:** Adjusts automatically to `App.DesignHeight - Self.Y`
- **Placeholder text:** Set via `Props.InputNewComment.PlaceholderText`
- **Styling:** Modify HtmlText controls for comment card appearance

## Internal Collections

| Collection | Purpose |
|------------|---------|
| `colCommentTable` | Stores parsed comments for display in gallery |

## Dependencies

- Uses `User().FullName` and `User().Email` for comment attribution
- Requires JSON parsing for loading existing comments
