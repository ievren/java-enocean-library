# Introduction #

The library acts in an event driven way.

The main entry point is the ![ESP3Host](https://code.google.com/p/java-enocean-library/source/browse/src/main/java/org/enocean/java/ESP3Host.java). You can find an example on how to use the library by looking at the ![Application class](https://code.google.com/p/java-enocean-library/source/browse/src/main/java/org/enocean/java/Application.java).

### Packet Reading ###
The !ESP3Host creates a new PacketStreamReader with the given ProtocolConnector. The PacketStreamReader reads the bytes from the stream and tries to parse a RawPacket which gets then parsed and converted to a BasicPacket (and sub classes).

### Packets ###
There are already various packet classes. Currently only RadioPacket classes are supported. Of them we use 1BS, 4BS, RPS and VLD.

### Data Parsing / EEP Parser ###
The packets itself do not know anything about their content. Only the !EEPParser knows how to parse the !Payload of the package. The !EEPParser are named after the device classes they support. A [List of all supported EEPs](SupportedDevices.md) can be found in the wiki.