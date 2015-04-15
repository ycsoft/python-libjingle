# Project Tapioca #

[Project Tapioca](http://tapioca-voip.sourceforge.net/wiki/index.php/Tapioca) is a component of Telepathy.  Tapioca, like libjingle and PyJingle, aims to be a complete API for instant messaging and P2P and it, in fact, includes an interface to libjingle and is not related otherwise to PyJingle. However, the API for Tapioca is different from PyJingle:

  * It aims to (some say schizophrenically) integrate IM, SIP, XMPP (Jabber), MSN, IRC, etc. in much the same way that Pidgin and libpurple do.
  * It's written C and C++, although it includes bindings for Python and C#.
  * It's designed to be a unified API of an amalgamation of technologies. Whether this is good or not, depends on what you're trying to do.

These are all good points if you're trying to implement a multitool client like Pidgin, but for something specifically geared at XMPP (Jabber) and Google Talk extensions, Project Tapioca has too many dependencies on other things to be a decent API.  Instead, you'll want to specifically just use libjingle.

So why create 'python-libjingle' when Python bindings for Tapioca exist? Well, if I have to explain this, you need to read this excerpt from [The Art of Unix Programming](http://catb.org/~esr/writings/taoup/) by Eric S. Raymond entitled [The Basic Unix Philosophy](http://catb.org/~esr/writings/taoup/html/ch01s06.html). Better yet, why not buy the book from [Amazon](http://www.amazon.com/exec/obidos/tg/detail/-/0131429019/104-5607387-8275944?v=glance), [Barnes & Noble](http://search.barnesandnoble.com/booksearch/isbninquiry.asp?endeca=1&ean=9780131429017), or [directly from the publisher](http://www.informit.com/store/product.aspx?isbn=0131429019)?