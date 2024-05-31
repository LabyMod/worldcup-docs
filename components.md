# Component Overview

This document provides an overview of all available components and their configuration options.<br>
A component consists of a sign with a specific text on it and a specific location.<br>
The text on the sign is used to identify the component and to configure it.<br>

**You need to have the WorldCup addon installed to use these components.**<br>
You can install the addon from the addons store **during** the event. Contact us if you want to get early access to the
addon.

## Component Structure

- **Namespace**: The namespace of the component, basically who registered the component. In this case it is the
  namespace `worldcup`.
- **Identifier**: The identifier of the component, this is unique for each component and determines the type of the
  component we want to place at a specific location.
- **Dimension**: Depending on the component type, the dimension can be used to set the size of a canvas that should be
  rendered above the sign.
- **Arguments**: Depending on the component type, different arguments can be passed to the component to configure it.

![sign](/.assets/sign_structure.png)

## Component Types

- [TV Stream](/components/stream.md)
- [List of Upcoming Matches](/components/matches.md)
- [Vote Station](/components/vote.md)
- [Effect](/components/effect.md)