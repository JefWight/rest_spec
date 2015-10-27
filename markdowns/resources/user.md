# User resource type

Represents an Azure AD user account. Inherits from [DirectoryObject].

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "Calendar",
    "CalendarGroups",
    "CalendarView",
    "Calendars",
    "ContactFolders",
    "Contacts",
    "Events",
    "Folders",
    "Messages",
    "RootFolder"
  ],
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "Alias": "String-value",
  "Calendar": {
    "@odata.type": "microsoft.graph.calendar"
  },
  "CalendarGroups": [
    {
      "@odata.type": "microsoft.graph.calendargroup"
    }
  ],
  "CalendarView": [
    {
      "@odata.type": "microsoft.graph.event"
    }
  ],
  "Calendars": [
    {
      "@odata.type": "microsoft.graph.calendar"
    }
  ],
  "ContactFolders": [
    {
      "@odata.type": "microsoft.graph.contactfolder"
    }
  ],
  "Contacts": [
    {
      "@odata.type": "microsoft.graph.contact"
    }
  ],
  "DisplayName": "String-value",
  "Events": [
    {
      "@odata.type": "microsoft.graph.event"
    }
  ],
  "Folders": [
    {
      "@odata.type": "microsoft.graph.folder"
    }
  ],
  "Id": "String-value (identifier)",
  "MailboxGuid": "Guid-value",
  "Messages": [
    {
      "@odata.type": "microsoft.graph.message"
    }
  ],
  "RootFolder": {
    "@odata.type": "microsoft.graph.folder"
  }
}

```
### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|Alias|String|The user's alias. Typically the SMTP address of the user.|
|DisplayName|String|The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates.|
|Id|String| Read-only.|
|MailboxGuid|Guid|The GUID assigned to the user's mailbox.|

### Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|Calendar|[Calendar](calendar.md)|The user's primary calendar. Navigation property. Read-only. Nullable.|
|CalendarGroups|[CalendarGroup](calendargroup.md) collection|The user's calendar groups. Navigation property. Read-only. Nullable.|
|CalendarView|[Event](event.md) collection|The calendar view for the calendar. Navigation property. Read-only. Nullable.|
|Calendars|[Calendar](calendar.md) collection|The user's calendars. Navigation property. Read-only. Nullable.|
|ContactFolders|[ContactFolder](contactfolder.md) collection|The user's contacts folders. Navigation property. Read-only. Nullable.|
|Contacts|[Contact](contact.md) collection|The user's contacts. Navigation property. Read-only. Nullable.|
|Events|[Event](event.md) collection|The user's events. Default is to show Events under the Default Calendar. Navigation property. Read-only. Nullable.|
|Folders|[Folder](folder.md) collection| Read-only. Nullable.|
|Messages|[Message](message.md) collection|The messages in a mailbox or folder. Navigation property. Read-only. Nullable.|
|RootFolder|[Folder](folder.md)| Read-only. Nullable.|

### Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get User](../api/user_get.md) | [User](user.md) |Read properties and relationships of user object.|
|[Create CalendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Create a new CalendarGroup by posting to the CalendarGroups collection.|
|[List CalendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) collection| Get a CalendarGroup object collection.|
|[Create Event](../api/user_post_calendarview.md) |[Event](event.md)| Create a new Event by posting to the CalendarView collection.|
|[List CalendarView](../api/user_list_calendarview.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create Calendar](../api/user_post_calendars.md) |[Calendar](calendar.md)| Create a new Calendar by posting to the Calendars collection.|
|[List Calendars](../api/user_list_calendars.md) |[Calendar](calendar.md) collection| Get a Calendar object collection.|
|[Create ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| Create a new ContactFolder by posting to the ContactFolders collection.|
|[List ContactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) collection| Get a ContactFolder object collection.|
|[Create Contact](../api/user_post_contacts.md) |[Contact](contact.md)| Create a new Contact by posting to the Contacts collection.|
|[List Contacts](../api/user_list_contacts.md) |[Contact](contact.md) collection| Get a Contact object collection.|
|[Create Event](../api/user_post_events.md) |[Event](event.md)| Create a new Event by posting to the Events collection.|
|[List Events](../api/user_list_events.md) |[Event](event.md) collection| Get a Event object collection.|
|[Create Folder](../api/user_post_folders.md) |[Folder](folder.md)| Create a new Folder by posting to the Folders collection.|
|[List Folders](../api/user_list_folders.md) |[Folder](folder.md) collection| Get a Folder object collection.|
|[Create Message](../api/user_post_messages.md) |[Message](message.md)| Create a new Message by posting to the Messages collection.|
|[List Messages](../api/user_list_messages.md) |[Message](message.md) collection| Get a Message object collection.|
|[Update](../api/user_update.md) | [User](user.md)	|Update User object. |
|[Delete](../api/user_delete.md) | None |Delete User object. |
|[Sendmail](../api/user_sendmail.md)|None||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->