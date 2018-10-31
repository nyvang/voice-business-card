# Vxml Business Card

This project is actually an old application I made back in 2013. 
When I was looking at the project again for a few weeks ago, I decided to create some documentation and to put the code on GitHub. I hope my little project can inspire and/or help someone create their own voice project.


## What does it do, and how?

As said, the application is a quite small file that describes some actions, which is read/run by a server at [Voxeo.com](voxeo.com).

You call a specific predefined phone number, which connects you the above mentioned server. All the functionality is provided by Voxeo as a service, and a great free service at that. 

The XML file contain some control statements with actions for the server to perform. These actions is provided to the user by a female voice. When the user answer, the server compare these with some text-to-speech (TTS) technology, acts accordingly and thus, we have a conversation with a computer. Fun, eh :metal:

### And the "how"

When started, the app reads some text from `<prompt>` element, to welcome the user and provide some simple instructions.
 
The xml file consist of a form with a single field and a list of input to this field.
The caller is informed of everything within the `<prompt>` element and meanwhile, the application listens for userinput. 
When input is detected, the voice recognition compare the `input` to the `if-elseif-else` statement where the correct input are listed.

### How to run the application?

There is quite alot of ways to call the application, and even some that uses SMS even though SMS is unsupported.

For this application, the following is supported:

 * International (Voice Only) - Denmark 
 * International (Voice Only) - Denmark
 * SIP VoIP
 * SMS Botkey
 * iNum Number (Voice Only)
