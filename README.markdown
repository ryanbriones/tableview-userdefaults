# TableView bound to User Defaults

This is based on code in a project I'm working on that SHOULD work based on "standard" IB setup I've seen. But, it doesn't work. It allows you to add a row, and edit it, but if you add new rows beyond that, all rows previous get wiped of data, even though the row count is preserved. Also, the row count, but not the data, is persisted across runs of the app. Very weird.

# The answer

"All you have to do to get it to work is check 'Handles content as compound value' on the array controller content array binding."
-- http://lists.apple.com/archives/cocoa-dev/2009/Apr/msg02114.html
