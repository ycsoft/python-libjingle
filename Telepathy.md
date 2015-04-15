# Telepathy #

Telepathy is a lower-level communications framework that is protocol, application, and platform agnostic.

![![](http://mission-control.sourceforge.net/mission-control.png)](http://mission-control.sourceforge.net/mission-control.png)

Where libjingle fits in is as a component library for the grey "Jabber" box.  python-libjingle is just a Python binding for libjingle.

Now for the $10000 question:  Where does ProjectTapioca fit on this diagram?  (Hint: it doesn't.  It would occupy the space between Telepathy and the four grey boxes.)

# PyJingle Relationship to Telepathy #

PyJingle would be a component library of the first grey box for Jabber/Google Talk:
  * A "Google Talk for Linux" would, ideally, be implemented as two components:  a UI, and the fully-fleshed out connection manager, though I suppose it could be one package that is a hybrid of the two.
  * Another project can provide a more Pythonic interface, between Telepathy Python and libjgingle.  This would be a connection manager, and a platform agnostic "Google Talk" client, occupying a "Chat UI" component could then be written using PyGTK, PyQt. wxWidgets, Jython and Swing, etc.
  * One of the existing UIs (Empathy, Kopete, etc.)  may adopt PyJingle or the above hypothetical project, but more like Tapioca in that it supports multiple protocols,(Grand Unified Messsaging for PYthon? ;) as part of a "plug-in" architecture for their software.
  * Pidgin has a Python interface.  Maybe someone could write a more complete plugin for libpurple and ties Pidgin into Telepathy, etc., but keep in mind that libpurple itself is not thread-safe.