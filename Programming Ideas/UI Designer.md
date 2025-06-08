# Idea
Make a UI designer that allows the user to use a graphical interface to create XML to use with builder.
# Points To Cover
- Text Generation: Need to be able to generate the XML text into a file
- Containers & Widgets: Needs to be able to create every type of container & widget, and manage their IDs
	- Allowing users to set IDs and auto generating IDs
	- Containers such as frames, windows, buttons, labels, ect
	- I also need to know all the settings for each widget/ container
- Main point is to function like glade, but with more modern features (and to support gtk4 in the future). These features are:
	- Auto alignment
	- A better UI
	- Draggable widgets
	- Every widget should be styled with CSS if styled at all. Allow user to manipulate CSS with the GUI or type CSS in themselves
	- Components & Pages can be represented in different UI files (Might be limited on this due to gtk)
- If this is done correctly, then following tutorials involving how to create UI using glade should translate over directly using my program.
# Accessibility
- Create a thorough documentation of each version
- Create videos for each documentation page & a small series on developing a basic app