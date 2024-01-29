The Carputer: A study in the design, construction, and implementation of a vehicle based computer system.

By: Je’aime Henri Powell

A Thesis submitted to The Director of the Honors Program and the Honors Council of
In partial satisfaction of the requirements for the Elizabeth City State University
Honors Program

February 4, 2004

Thesis directed by
Director of the Honors Program Carol C. Jones
Kristna Kulkarni and
Computer Science Professor


# The Carputer:

## A study in the design, construction, and implementation of a vehicle based computer system.

### Created by: Je’aime H. Powell


## Introduction

The purpose of this thesis is to detail the conception, design and implementation of a
computer into a stock 1998 Dodge Neon vehicle. The final Carputer will consist of a
standard ATX style computer capable of running a DIVX player, an mp3 player, game
emulators, Windows 98, desktop publishing software, and both passive and active LCD
displays. The final stage of the Carputer will also have a custom designed controller for
driver use. To tie all software together, a custom operating system shell will act as a
menuing system to integrate all uses of software.

This thesis will not cover advanced circuitry design, advanced programming techniques,
or advanced software use techniques. Third parties to whom this project has no affiliation
will have created some components and software. Due to this fact detailed schematics
and or source code may not always be available. This thesis is a study in the integration
of available equipment, materials, and software, not the creation of a Carputer from raw

## materials.

## Components

The function of the Carputer is driver / passenger entertainment. Unlike car computers
used to control fuel-air mixtures or interior temperatures, the Carputer allows music,
movies, navigation, games, and any other function a standard home computer could
provide. The Carputer will be composed of a variety of individual components to create


one seamless unit. This unit will control all aspects of entertainment in the vehicle. This
chapter will break the Carputer into its individual parts including processing, input,
output, software, and the custom dash.

## Processing

The Carputer will actually contain the components of a modified desktop computer. The
initial stages of the Carputer will use a socket 7, 200mhz motherboard and chip to do
basic implementation testing. Although the 200mhz processor does not have the power to
push DIVX type movies or game emulation, it does allow basic power and hardware
concepts to be explored. The final stages of the project will use a ~500mhz, socket 370
processor and motherboard to allow DIVX / DVD movies and Game Emulation to run
while having extra system resources available for future system upgrades.

Stages one and two of the Carputer project will both utilize the moderately older socket 7
system architecture for testing. The socket 7 architecture was the elite computer platform
of its time. Socket 7 allowed desktop computers reach speeds of 100mhz, which was a
great leap from then current speeds of 66mhz. This architecture also saw the birth of the
Intel Pentium processor, which soon became a household name. The mainstreaming of
64bit, PCI (Peripheral Component Interconnect) slots also became a computer standard
thanks to the socket 7, 66mhz bus speed (Bus speed is the speed which a processor
communicates with its RAM and motherboard peripherals). This change allowed the term
"Plug and Play" to become a permanent stamp on the brain of any computer hardware


purchaser. Plug and Play gave hardware the ability for components to not only function,
but also have imbedded instructions that allowed computers to identify devices pre-driver
installation. The socket 7 system architecture’s last hurrah was the development of the
AMD K6-2 / 3d Now! platform. This allowed the socket 7 to soar to the theoretical limit
of 550mhz. This dream was short lived because of the ancient 100mhz max bus speed
limitation and no on processor cache. Cache is fast memory or registers holding recently
accessed data, designed to speed up subsequent access to the same data. This lack of
cache made the processors run new multimedia rich software extremely slowly. The
newer 133mhz and 266mhz bus speed processors swiftly gained market share and the
Socket 7 motherboards and processors faded into computer history. The socket 370
platform used for Stages three and four will have a bus speed of 133mhz and a processor
speed of ~500mhz. The processor will also have a 512k cache and 128mb of RAM
(Random Access Memory) to allow the Carputer to multitask with out hesitation. RAM
is an integrated circuit memory chip that allows information to be stored or accessed in
any order, and all storage locations are equally accessible.

To aide in the understanding of RAM, cache, and hard drive memory in reference to the
processor think of a worker in an office. The worker is the processor to this office
computer, getting and using information. The file cabnents in the office are like the hard
drive of the computer. The more cabinets had, the more files or information that can be
stored for long periods of time. The problem is that every a file wanted, the worker has to
physically get up and get the files from the cabinet. This makes this type of memory very
slow. RAM improves this function by acting as an in/out boxes on the desk. What is in


the boxes is known because they are so small and have been recently used. Also the more
in/out boxes possessed, the quicker information can be used by the worker. In computer
terms RAM is digital storage that is cleared every time the computer is restarted or a
program is closed. Then there is cache. Cache is like having a file in the workers hand.
The information is readily available but, upon not needing the file, it returns the file to
either the in/out box (RAM) or the file cabinet (hard drive). The way these three items
interact with each other, and other devices in a system determines a computer systems’
overall speed and system resources.

## Power Conversion (~12VDC to ~120VAC)

The most inherent problem with installing a fully functional computer into a vehicle is
that of power. A computer motherboard only uses a max of ~12VDC (Volts Direct
Current) which is the same amount of volts a standard car battery and alternator send (or
~13VDC with the alternator charging). The problem is the fact that a computer uses very
specific amperages and voltages which if not maintained can plague a computer with
lockups and/or damage. The most direct response to maintain the correct wattage and
voltage is to use a standard ATX (Advanced Technology Expansion) computer power
supply unit (PSU). The obvious problem this decision creates is how to take the ~12VDC
from a car battery and change it to ~120VAC (Volts Alternating Current) for a standard 250 watt ATX power supply?


The answer to this question came in the form of a device called a power inverter. An
inverter is an electronic component used in digital systems that takes the logical value of
its input and complements it. So, if the input voltage is logically low, a high voltage
appears on the output, and vice versa. The exact values of the high and low voltages
depend on the semiconductor family. (jakohn, (2000,April). inverter. Everything2 (On-
line), [http://www.everything2.com/index.pl?node=inverter)](http://www.everything2.com/index.pl?node=inverter)) Hence, a ~12VDC car power
connection can be inverted to ~120VAC. The one other question is one of wattage. With
a power supply pulling ~250 watts a matching or greater wattage will be needed to
prevent brownouts. From stage two until stage four, a 300watt / 600watt peak inverter
will be used in order to run the Carputer stably.

When deciding upon a power inverter for the Carputer, building one from scratch was
first considered. Although this is viable and very economical, the side effect of one bad
solder could be a burned motherboard. After much consideration it was decided to
purchase a 300-watt pre-built inverter. On the plus side of purchasing a power inverter is
the fact that the inverter comes with a heat sink large enough to disperse the access heat
evenly. The fact that the inverter will have a manufacturers warranty as a guarantee is also a great control when variables are in abundance in this project.

## Input

The Carputer will have a mixture of both traditional and modified input devices through
out its stages of development. From a standard keyboard and a mouse to a modified game


pad and a touch screen, peripheral inputs will allow the user of the Carputer to easily use
software in the Carputer with out compromising control or safety of the vehicle while
driving.

Stages one through four will use a standard keyboard for peripheral data input however in
stage two a standard keyboard control module will be modified in order to add the ability
to quickly access certain functions in the Carputer’s shell. Certain key presses will be
hard wired from the keyboard module into on/off momentary push switches to allow the
user easy access to hot key functions (i.e. for WinAmp, Play, Pause, Stop, and Skip
Next). These switches will mount into the custom dash in stage four to not only look
attractive but also functional.

Windows 98 often needs a mouse to perform standard tasks easily. The mouse that will
be used in the Carputer is a small form mouse called a "Thumb Mouse." This mouse fits
like a ring between the users index finger and thumb. The thumb will control x and y axis
movements while the index finger uses a trigger type switch to "left-click" in windows.
The thumb mouse will be used just like a regular mouse for easy access to functions in
the operating system or Carputer shell. In Stage four of the project, a second mouse will
be installed directly on the TFT LCD display. This second mouse will actually be a touch
screen membrane that will allow mouse like actions to take place by simply pointing to
the area on the screen with the desired action.


Touch surfaces are created by coating a flexible plastic (optical quality polyester) film
and chemically hardened glass with a nearly invisible super-thin layer of metal. These
two surfaces are separated by extremely small transparent separator dots, which act like
insulating springs, maintaining an even distance between the two metallic coated layers.
A small electrical current of 4-6 volts DC at less than 60 milliamps is passed through the
metallic-coated
layers. When
pressure is
applied to the
surface, the
separator dots
allow the two
charged surfaces
to make contact.
The resultant signal is then sent to the controller box, which determines the exact point of
contact and registers the "touch" as a mouse would register a "click".

The final form of input into the Carputer is that of a standard game pad. This game pad
will be connected through the soundcard's MIDI / Game Port. The game pad will be used
primarily to control games while in the emulator. The game pad module can also be
modified to allow control of WinAmp for MP3 playback. Though this function will in all
likelihood not be used, it could be a third form of control. The game pad is an input
device that only the passenger will be able to enjoy during travel.

```
(Provided by: http://www.ezscreen.com/technology.html)
```

## Output

All of the stages of the Carputer will have either a parallel LCD (Liquid Crystal Display)
and/or a TFT (Thin Film Transistor) LCD. A liquid crystal display is a type of display
used in digital watches and many portable computers. LCD displays utilize two sheets of
polarizing materials with a liquid crystal solution between them. An electric current
passed through the liquid causes the crystals to align so that light cannot pass through
them. Each crystal therefore is like a shutter, either allowing light to pass through or
blocking the light. There are two types of LCDs, active matrix and passive matrix.
Passive matrix LCDs are commonly used in watches, older cell phones, and any other
two-tone LCD displays. Passive matrix is the simplest form of LCD display. Active
Matrix or TFT LCDs are often found in Laptops, LCD Display Panels, and in color cell
phone displays. TFT LCDs have transistors on the back of each photoelectric cell to
allow controlled fading times. This allows CRT (Cathode Ray Tube) quality display. An
LCD that can show colors must
have three sub pixels with red,
green and blue color filters to
create each colored pixel.
Through the careful control and
variation of the voltages applied,
the intensity of each sub pixel
can range over 256 shades. Combining of the sub pixels produces a possible palette of

```
(Provided by:
http://electronics.howstuffworks.com/lcd5.htm)
```

16.8 million colors (256 shades of red x 256 shades of green x 256 shades of blue), as
shown below. These color displays take an enormous number of transistors. For example,
a typical laptop computer supports resolutions up to 1,024x768. The product of 1,
columns by 768 rows by 3 sub pixels equals 2,359,296 transistors etched onto the glass.
Stages one through four will use a passive HD44780 LCD controlled by a parallel port
interface to display song titles, system speed, and any other text-based system
information. Stages three through four will use a TFT LCD to display complex
visualizations and the operating system shell.

During Stage two of implementation the Carputer will actually function within the Dodge
Neon. Standard computer speakers would waist valuable inverter power as well as would
not look very attractive in the vehicle. Initially this problem will be overcome by simply
using a Phono to cassette adapter in the car's stock radio. Though a "quick fix" this is not
the most attractive or inclusive addition to the vehicle.

Stage four will remove the stock car radio and replace it with the Carputer. The two
problems inherent with removing the car radio are number one: volume control, and
number two: amplification. A standard computer sound card relies on self-amplified
speakers to push out sound. If a standard sound card were connected to the six non-
amplified speakers in the neon even at the sound cards highest volume, the sound would
come out as a whisper. For the Carputer to provide good, clean sound an amplifier will be
used.


Any car radio aficionado says speakers determine what wattage an amplifier must be.
Due to the fact the Neon will still have the stock speakers and stereo, Dodge specs can be
followed to determine the power and number of channels needed to get the best sound
quality. According to Dodge the 1998 Neon has a six-speaker system. These speakers by
classification are: two high range speaker (tweeters) in the front dash, two mid range
speakers (mids) in the door panels, and two low-range speakers (subs) in the rear of the
car. Per Dodge, each speaker should receive no more than 15 watts to 20 watts of power.
The actual stock radio in the Neon pushes 120 watts to four channels. Each channel
normally carries one speaker however there is a crossover in between the two front
speakers and the radio. This crossover serves two purposes. Number one the crossover is
"high-pass" which means it blocks low frequencies as to not damage the high range
speakers. Number two; the crossover ties the front tweeters and door mid-ranges together
on the left and right channels.

As far as the radio is concerned there are only four channels connected; Front Right,
Front Left, Back Right, and Back Left. Though these four channels could be split into six,
in sticking with the stock sound concept, removal of the crossover would be unwarranted.
Moving to a six-channel system would also undermine the four-channel Sound Blaster
Live! sound card.

The reason the Sound Blaster Live! Soundcard is planned for stage four implementation
is because of the extreme sound quality the card produces, and the fact that the card has


four-channels. The Sound Blaster Live! brings cinema-quality sound to movies, music,
and games with digital 5.1 clarity. Driven by the powerful EMU10K1 Digital Signal
Processor, the listener experiences the highest-quality sound reproduction with real-time
audio and effects. The Sound Blaster Live! makes it fast and easy to create, customize,
and listen to quality MP3/WMA files. With the ability to connect to Dolby Digital and
multi-channel digital speaker systems or analog audio devices, true 5.1 surround sound
can be experienced with all PC audio entertainment (Jupitermedia Corporation (2003)
Creative Labs Sound Blaster Live 5.1 Sound Card Sound Card: Overview. Hardware
Central: (On-line), [http://hardwarecentral.dealtime.com/xPO-](http://hardwarecentral.dealtime.com/xPO-)
Creative_Labs_Creative_Labs_Sound_Blaster_Live_5_1_Sound).

A quick tour of the sound path from the Carputer to the speakers will help illustrate how
the amplification will fit in with the project. First
the sound will synthesize through the Sound
Blaster Live!. This sound will be non-amplified
but extremely clear. The non-amplified sound will
then be split into the four channels of front left,
front right, back left, and back right. The four
channels will then feed in to a ~120 watt amplifier
to push the speakers. The back two channels will
go from the amplifier directly into the left and
right subs. The front two channels will lead off
the crossover where the two left and right channels becomes four channels which will


then lead to the left and right tweeters, and the left and right mid-range speakers. The
~120 watt amplifier will not make this system a "blasting" system however; the quality of
the unit will be outstanding.

## Operating System and Software

The Carputer will use Microsoft Windows 98 as its core OS (operating system). The OS
is the low-level software, which handles the interface to peripheral hardware, schedules
tasks, allocates storage, and presents a default interface to the user when no application
program is running. The reason Windows 98 will be selected as the main OS instead of
any of the other versions of Windows or even Linux, is due to the fact that windows 98
has USB support without the bloat-ware of Windows ME or Windows XP. As far as
Linux, support is almost not present to the everyday user.

Microsoft Windows 98 is the third generation of the windows platform. Proceeded by
Windows 1x, Windows 2x, Windows 3x, Windows NT, and Windows 95. Windows 98 is
at the pinnacle of its times technology according to Microsoft:

"Windows 98 was the upgrade from Windows 95. Described as an operating system that
"Works Better, Plays Better," Windows 98 was the first version of Windows designed
specifically for consumers.


With Windows 98, users could find information more easily on their PCs as well as the
Internet. Other ease-of-use improvements included the ability to open and close
applications more quickly, support for reading DVD discs, and support for universal
serial bus (USB) devices (Microsoft (2003, June). Windows Overview & History.
Windows Products and Technologies History: (On-line):
[http://www.microsoft.com/windows/WinHistoryIntro.mspx)."](http://www.microsoft.com/windows/WinHistoryIntro.mspx).")

The backward compatibly of Windows 98 allows the use of older equipment if necessary
while most new equipment is compatible also. This will allow the Carputer to have
scalability. The most obvious implementation of this feature is the fact that stage one will
use an old Pentium 200mhz processor and board while stage three will use a Socket 370
architecture. The transition from old architecture to new will be smooth thanks to the OS
integration. Windows 98 is also new enough an operating system that DIVX software and
playback is compatible while at the same time DOS Support is available if needed.

Though Windows 98 will be the "back-bone" of the Carputer system, other third party
drivers and software will allow the Carputer to play movies, play music, and play games.
The Carputer will also have a master menuing shell, which will allow easy access to all
of the Carputer’s functions. The way all of these separate programs integrate will make
the difference between a feasible entertainment system and a high end-tech toy.


The original idea behind the Carputer was to play music in the MP3 (Moving Picture
Experts Audio Level 3) format. MP3 is a digital audio compression algorithm that
achieves a compression factor of about twelve while preserving sound quality. It does this
by optimizing the compression according to the range of sound that people can actually
hear. MP3 is currently (July 1999) the most powerful algorithm in a series of audio
encoding standards developed under the sponsorship of the Moving Picture Experts
Group (MPEG) and formalized by the International Organization for Standardization
(ISO). MP3 files are usually downloaded completely before playing but streaming a MP
is also possible. A program called a "ripper" can be used to copy a selection from a music
CD onto a hard disk and another program called an encoder can convert it to an MP3 file
(http://www.hyperdictionary.com). The player for the encoded MP3 files in the Carputer
will be WinAmp due to the versatile nature of the program.

WinAmp itself has a very interesting history beginning in the mid 1980's. Fraunhofer
Institute in Erlangen, Germany, which began work on a high quality, low bit-rate audio
coding with the help of Dieter Seitzer, a professor at the University of Erlangen. In 1989,
Fraunhofer was granted a patent for the MP3 in Germany and a few years later it was
submitted to the International Standards Organization (ISO), and integrated into the
MPEG-1 specification.

In the early 1990s the first MP3 player was developed, however it was such a huge file,
that it could not be used. In 1997 a developer at Advanced Multimedia Products named
Tomislav Uzelac created the AMP MP3 Playback Engine, which is regarded as the first


prime time MP3 player. Shortly after the AMP engine hit the Net, a couple of university
students, Justin Frankel and Dmitry Boldyrev (who more recently created Mac AMP),
took the Amp engine, added a Windows interface and dubbed it "WinAmp" (Garcia,
Daniel. The Origin of the MP3 (On-line):
[http://www.uweb.ucsb.edu/~dgarcia/Origin/origin.htm).](http://www.uweb.ucsb.edu/~dgarcia/Origin/origin.htm).)

DIVX will allow the Carputer to play saved movies directly from the hard drive. This
will take away the problem of scratching DVD discs and cluttering up the car. DIVX has
had a very diverse history also, starting out as a commercial venture with Circuit City.
Originally known as Zoom TV, DIVX was a home video system originally conceived
around 1994 by prominent Los Angeles entertainment law firm Ziffren, Brittenham,
Branca and Fischer. They teamed up with Circuit City Stores, the largest consumer
electronics retailer in the U.S. at the time, to develop the idea into a marketable product.
DIVX the name was derived from the company's name of Digital Video Express L.P.

DIVX was based on DVD-V, and boasted high-quality MPEG-2 digital video and Dolby
Digital surround sound. Unlike DVD, which was an effort to exploit the growing sell-
through video market, DIVX was a rental system, perhaps the most sophisticated ever
offered to the public, that allowed near video-on-demand, with no late fees and the
availability of many "hot new release" rental titles day and date with their VHS
equivalents. DIVX was officially announced in September 1997; about 6 months after
nationwide marketing of DVD players began. DIVX, however, wasn't released to test
markets until June of 1998, and nationwide a few months after that (Dunnill, R.J. (2003).


A Short History of the Divx Home Video System. DIVX Owner’s Association: (On-line),
[http://www.the-doa.com/Pages/DoaDivxHistory.html).](http://www.the-doa.com/Pages/DoaDivxHistory.html).) Unfortunately customers decided
to own DVDs rather than rent DIVX Discs so Circuit City canceled the project in June of

2001. Customers where left to fend for themselves until an innovative programmer
named Jérôme Rota reinvented DIVX in the world known CODEC it is today.

For the high-tech community, he is the French kid, the guy making Hollywood sweat
with an invention called DIVX;-), an increasingly popular underground program known
as "the MP3 for video." For Microsoft, he is the hacker who “stole” elements of their
technology to create a method for people to illegally pirate movies over the Internet. In
France, he’s the media darling from the Mediterranean city of Montpellier, who had the
nerve to take his ideas to Southern California and launch a company he brazenly called
"Project Mayo." Gej, also known as Jérôme Rota, describes himself simply as “a video
lover.” “The rest of the DIVX;-) story is an accident,” he says in a musical Southern
French accent, from Project Mayo's offices in La Jolla. Back in Montpellier Gej was
working as a 3D graphic artist for firms such as Lancôme, and he wanted to archive his
clips. “Not on a VHS tape, but on CD-ROMs, for a more beautiful quality and a cleaner,
durable result.” Drawing on nearly 20 years experience programming and tinkering with
computers (at age 8 he was already breaking his piggy bank to buy machines and parts),
Gej put together a hybrid program based on Microsoft and MP3 technology.

The resulting "DIVX;-) (An ironic reference to the failed movie-disk format DIVX)
allows high-quality digital video files to be stored at 15% of the size they normally


require. As soon as Gej posted the program on an Internet Relay Chat (IRC) network,
video fans bombarded him with e-mails. Gej told himself, “I will build a website and post
it there, and hopefully I won’t be bothered anymore.” The site received 40,000 visits the
very first week. “It just exploded,” he said. (Richard, Emmanuelle. (2000). Jérôme Rota,
co-founder of Project Mayo, La Jolia, Architects and Pioneers 2000: (On-line),
[http://www.emmanuellerichard.com/Articles/ArticleScanBIS/Articlesscan/divx.htm).](http://www.emmanuellerichard.com/Articles/ArticleScanBIS/Articlesscan/divx.htm).)

Jérôme Rota actually used name recognition to boost the use of his DIVX;-) Codec.
Although based on the same theory of video on demand, the DIVX;-) codec has very
little to do with the original DIVX home video system. The interesting part of the DIVX
history is that the original DIVX had corporate backing and millions of dollars behind it
yet Jérôme Rota's DIVX;-) codec was just the dream of a young man to save DVDs to his
computer. The DIVX;-) codec is now one of the most downloaded file types on the
Internet today.

The Carputer will also use a DVD-ROM drive and decoder card to play DVD movies and
CD discs. When CD-ROM was developed over 10 years ago, it had the ability to store
over 650MB worth of data or 70 minutes of music. At the time, this capacity seemed
almost unlimited. Most users never dreamed they would require over 650MB. Ten years
later, the industry and consumers are pushing the 650MB barrier. Many of today's
applications call for well over 650MB of storage. Currently, the only options available to
address these needs are compression schemes or the use of multiple discs. Each one of
these solutions has its drawbacks. Therefore, a second-generation disc technology was


needed to address today's high amount of data requirements for video, multimedia,
database, etc. That new technology is DVD.

Early in 1995, two major groups were competing to develop the next generation of high-
density compact disc. Under the partnership of Philips and Sony, there began the
development of one such format. Concurrently, a group led by Toshiba and Time Warner
was working on another format. At one point, it looked like the two groups would each
bring to market separate high-density compact disc solution. This would have been
analogous to the battle of Beta versus VHS in the home videotape recorder industry.
Another battle of this type would have adverse consequences for both the industry, as
well as the consumer. Fortunately, in September of 1995, the two camps agreed to
develop a single standard for a high-density compact disc.

In December 1995, the two groups agreed on the official name and most of the
parameters governing the new high-density compact disc. The name that was agreed
upon for the new high-density disc was DVD, which was not originally intended to be an
acronym. However many people refer to DVD as the Digital Versatile Disc or Digital
Video Disc. It should be noted that discs for the new DVD movie players are being
referred to as DVD; whereas the discs for the computer drives are being referred to as
DVD-ROM. The agreement took parts from both Sony/Philips and Toshiba/Time
Warner's former separate proposals and combines them into one. The "best practices"
compromise includes Sony/Philips' EFM-plus data storage scheme as well as backward
compatibility with current CDs. In other words, the new DVD and DVD-ROM players


must be able to play today's current CDs.

From the Toshiba/Time Warner side; the new DVD standard adopted their format of
using two half-thickness (0.6mm) discs bonded together for a double-sided disc. The new
standard also allowed for 3M's dual layer "2P" technology to be used.
Therefore, the new DVD discs can store from 4.7 GB (single sided, single layer) up to
17.0 GB (double sided, dual layer per side for a total of 4 layers of information). Each
layer of data on a DVD disc will allow up to 133 minutes of full motion MPEG-2 video.
This amount of playing time will allow 95%
of all movies to be contained on one side of
a disc. This new disc will also support a
variable bit data rate that increased the
quality of digital video playback thanks to a
substantial buffer memory. The new DVD
movie players are also capable of seamless
switching between the two layers of
information on each side of the disc (Bellwelther Manufacturing. (2003). DVD
HISTORY & BACKGROUND INFORMATION: (On-line),
[http://www.bellwethermfg.com/bellwether/dvd/dvdhist.htm).](http://www.bellwethermfg.com/bellwether/dvd/dvdhist.htm).)

Due to the fact that the Carputer is a fully functioning computer, game system emulation
will allow passengers to enjoy video games during travel. TFT LCDs unfortunately have
very low refresh rates, which mean in lay terms that high graphics games will not look

The following is a summary of the most
common DVD capacities:

- 4.7 GB (Single Layer Single Side)
- 8.5 GB (Dual Layer Single Side)
- 9.4 GB (Single Layer Double Side)
- 17.0 GB (Dual Layer Double Side)


good on the screen. Older games on the other hand look great at lower refresh rates. For
this reason the Carputer will incorporate older 16-bit games from the Nintendo and Sega
console era. These games will run through a program called an emulator. Emulators are
software versions of hardware-based consoles. These emulators use ROMs (Read Only
Memory) of video games to simulate console play. The Carputer will have two separate
emulators, one for the Nintendo and one for the Sega Genesis systems, which will each,
have hard drive saved ROMs for game play.

One of the main sources of integration for the Carputer will be the custom written shell
menuing system. This system will allow easy access to all main functions of the Carputer
by the user. The shell will actually be created in macromedia flash to allow user-friendly
menu changing options, and also the flash format can run as an executable file without a
player. This menu will be brightly lit with well-defined text fonts and sizes. The only
graphics used will be the picture of the car itself. The reason this menu needs to look so
clean is for quick recognition of functions. In other words the user (especially the driver)
needs to glance and select the desired function with out trying to focus on small or fancy
font types. The implementation of this shell into the operating system will help add both
safety and functionality to the overall Carputer project.

## Custom Car Interior

Stage four of the Carputer will have an installation of the completed unit into the Neon.
The installation brings about several problems to which only a custom dash is the


solution. The custom dash will actually contain the completed system with both LCDs,
the modified keyboard control, DVD-Rom, Hard drive, and Motherboard. The current car
radio will be removed and the part of the dash that the radio, ashtray, and lighter are
mounted into will be cut out. This area will be replaced with a 1/4" plywood dash box.
The dash box will be coated with stain and polyurethane to look attractive. The TFT will
be recessed at an approximate angle of 45° to allow easy viewing of the screen by both
the passenger and the driver. The screen will also have easy access for use of the touch
screen features. Having the screen under the cover of the dash also prevents windshield
reflection at night. This modification of the dash will be radical but the additional space
will allow better incorporation of the Carputer. There are two negatives to this form of
modification. One: the modification will be a permanent change to the neon interior and
two: the cup holders will be removed.


## Initial Planning

Prior to the completed version of the Carputer was envisioned, there were a few
prototype designs that gradually grew into the final design. This chapter will explore a
few of these original designs to show how research changed the unit into a much more
useful addition to the vehicle.

DOS-Based MP3 Player

The original design of the Carputer was to use an older Pentium style computer to simple
store and play MP3's through the car stereo. Originally the unit did not have a hard drive,
it only had a floppy to boot the operating system and a CD-ROM to play burned MP3's.
KIS (Keep It Simple) was the "order of the day" when it came to the design of this unit.
As simple as the original design seemed, it stemmed many questions such as display,
storage and power continued to arise.

The first step in this design was to find a program, which could play MP3's in DOS. After
much research a program called "DAMP" created by Matt Craven in the United Kingdom
was found. DAMP was a free MP3 player for DOS, which not only allows the playback
of MP3 files, but also the visualization of the audio through responsive image
manipulation. Not just "here's a pretty pattern", but images that respond to the audio in
order to create a richer, more fulfilling experience (http://www.damp-mp3.co.uk/). As the
DAMP website says, "DAMP also contains many of the features you'd need in an in-car


MP3 player or jukebox." As for the Socket 7 200mhz processor, DAMP had been
tested using a "486 DX4 100MHz with ESS Card and 12MB RAM." To say the least, this
program was a custom fit for a DOS-based mp3 player.

DAMP only had one inherent flaw; it did not change frequencies on the fly. This means
that if the first MP3 plays at a high frequency and the next is a low frequency, the second
MP3 would sound terrible. Though the MP3 sampling frequency could be altered before
use with the player, that would cause a lot of extra work when this function is automatic
in windows based players.

The original design called for the use of CD-ROMs to store mp3's. It was decided CD's
have a few too many flaws such as, scratches, in car storage areas, and skips during play.
To counteract these problems it was decided to use USB flash memory. Usually USB
ports are not supported in DOS however there is a third party driver called
"USBASPI.SYS" ("Panasonic v2.06 ASPI Manager for USB mass storage")
(http://www.freedos.org/freedos/news/newsitem/149.html). This driver would allow USB
connected digital media to hold the MP3's. Due to the fact that the storage media would
be digital, there would be no scratches to worry about, no storage issues, and no skips in

```
(DAMP Screen shot provided by: http://www.damp-mp3.co.uk/)
```

music while traveling over bumps in the road. The only draw back to this form of storage
was that the computer would have to boot from floppy. The only question this left is how
to view what the computer was displaying.

To tackle the display problem it was decided to go low-tech. Installing either a CRT
monitor or LCD Panel seemed totally unfeasible with both size and cost. After searching
through some old computer cases an old server case was found, which had a lighted LCD
screen to display simple system information. After "junking" the case it was found that
the chipset number on the back of the LCD screen was HD44780-8A. After some
research on the Internet it was found that these screens were often modified to connect to
parallel ports to in fact display system temperatures, disk space and MP3 identification
(Id) tags. This meant that this LCD would suite the needs of a Carputer perfectly except
for one slight issue. The parallel driven display would not give any type of information
on whether the system was booted or if there was some type of system issue. In other
words if something went wrong during boot up or while the computer was running there
would be no sign that it had happened. In looking into ways of redirecting the DOS
output to the parallel port however, the LCD driver and API (Applications Program
Interface) would not allow direct input from the command line.

## Display Issues

As this issue was researched it was found that this very issue became the focus of many
other such creators. What many creators decided to due to combat this issue was to use a


system that simply did not crash, such as Linux. To attempt this road less traveled Linux
was installed and tested as a viable solution. After much testing low support for the rebel
operating system made this route unfeasible. Some creators simply stuck to the parallel
LCD route and hoped all would go well with a windows based system. Many failed due
to the inability to deal with problems as they arose on the road. Others purchased $300+
in dash car LCD panels. This was very uneconomical. Once again used parts were leaned
to find an answer. Thanks to Joel Hathaway an old Dell Laptop was offered up.
Unfortunately the computer itself was fried but the 12" TFT LCD Screen was perfect.
This screen would not only allow standard output for the computer, but the computer
could also use a Graphical User Interface (GUI) instead of text-based output. This one
revelation opened the door for the MP3 Player to become a Carputer.

During the research of the actual conversion from laptop use to computer use it was
found that LCDs are controlled completely differently that a standard VGA Monitor. A
standard LCD panel takes input and converts it to a digital sequence that only TFT LCDs
use. This digital output controller searches screen refresh data for consistent colors in
order to only change the pixels that need to change. The problem in the Carputer case and
this form of technology is the controller which can cost as much as $200.00. This is a
problem, which still must be tackled through further research during construction.

The shear size of the TFT LCD has also caused a problem with space. The original DOS-
based player used a small LCD display, which could have sit on the dash. The 12" TFT
would create a huge blind spot if mounted to the dash, which would impede driving


views. If the TFT was mounted in front of the dash is would cover all radio controls and
environmental controls. A side console mount would impede the space of the passenger.
The only viable solution is to modify the dash itself.

The sear size of the 12.1" LCD screen will make its implementation unwise,
uncomfortable, and unsafe. Full functionality was still wanted from the computer so
another TFT solution was searched for. The answer came in the form of a 5.1" video
game system LCD Screen. The screen will cost approximately $70.00, which is well in
the range of money allotted in the budget for the project. The Sony Playstation uses the
RGB output format to make the unit portable. The LCDs, which connect to the
Playstation’s, have built-in controllers, which will allow for easy modification for
computer SVGA (Super Video Graphics Array) use. Because the LCD has the same
RGB, Horizontal Sync, Vertical Sync, and Ground that a standard video card has, all the
modification will need is an old VGA cable use as the connection.

```
(Provided by: http://mpro.no-ip.com/lcd2.htm)
```
## Dash Modification Design


Currently the dash has an area of 9"X 10.5" X 6” as the area for the radio, environmental
controls, and ashtray. The average size of an ATX motherboard is ~12" X 10". The size
of the TFT LCD Panel is 5.1" X 5". These measurements left a great disparity between
size of the project and actual usable space. One solution is to mount the computer itself in
the backseat or trunk. The inherent problem with a design like this is changing DVD's or
CD's. To solve this overall problem in one step it was decided to build a custom dash,
which will house both the TFT LCD and completed unit. This dash will be constructed of
.25" finished plywood. The TFT will sit at an approximate angle of 45 degrees. The TFT
will be recessed under the dash to prevent windshield glare during night use. The angle
will also make a touch screen a welcome addition to the Carputer, as it will allow easy
access for the driver. The dash went completed will have a dark stain and multiple layers
of polyurethane. If done correctly the wooden dash will be an attractive yet functional
addition to the vehicle. The negative to this design is the fact that the finalized product
will be permanent.

## Stages Breakdown

In order to accomplish all of the goals of the project, The tasks were broken down into
stages. Each stage will have specific goals to be accomplished. There will be four stages
starting with basic software control and ending with stage four, which will have the
completed unit, installed into the vehicle with dash modifications.


Stage One:
Stage One Objectives:

- Socket 7 Sytem construction
- Initial Software Implementation
    (WinAmp, Windows 98)
- Parallel LCD Construction and testing
System Specifications:
- Pentium 200mhz Processor on
    Socket 7 Motherboard
- 32mb RAM
- 5.1 GB Hard drive
- CD-Rom
- AT Case
- 17" CRT Monitor
- AT Keyboard
- Serial Mouse
- Standard 2 Speakers - Channel Amplified
- HD44780 LCD Display

Stage Two Objectives:

- Implement power inverter.
- Construct a custom keycontroller. board
- Use the computer within the
    vehicle.
- Modifycustom controller. WinAmp for use with the
- Use the cassette to Phono adapter
    for sound.

(^) System Specifications:

- Pentium 200mhz Processor on


```
Socket 7 Motherboard
```
- 32mb RAM
- 5.1 GB Hard drive
- CD-Rom
- AT Case
- AT Keyboard
- Thumb mouse
- Standard 2 - Channel Amplified
    Speakers
- HD44780 LCD Display

Stage Three
Objectives:

- Construct and
    implement a TFT LCD
- Construct ATX based
    Socket 370 system
- Implement version 1 of
    the Carputer Menuing
    Shell

(^) System Specifications:

- VIA C3 GigaPro
    Processor
- 128mb RAM
- 5.1 GB hard drive
- Socket 370 based motherboard with
    sound and video
- PCI based TV tuner


```
and Radio card
```
- DVD-Rom
- HD44780 LCD (Secondary display)
- TFT LCD (Primary
    display)
- Custom Controller (Primary Input)
- Windows 98 with
    Carputer Shell
- Thumb mouse (Secondary input)
- PS/2 Keyboard
    (Secondary input)

(^)
Stage Four
Objectives:

- Construccustom dasht and install
- Install amplifier to stock
    vehicle speakers
- Connect TV tuner / Radio card to car antenna
- Connect Carputer to
    amplifier
- Install Touch Screen and configure
- Implement and test
    Carputer Menuing Shell
version 2^
System Specifications:


- VIA C3 GigaPro
    Processor
- 128mb RAM
- 5.1 GB hard drive
- Socket 370 based
    motherboard with sound and video
- PCI based TV tuner and
    Radio card
- DVD-Rom
- HD44780 LCD
    (Secondary display)
- TFT LCD (Primarydisplay)
- Custom Controller
    (Primary Input)
- Windows 98 with Carputer Shell
- Thumb mouse
    (Secondary input)
- PS/2 Key(Secondaryboard input)


## Stage 1:

Objectives:

1.Socket 7 System Construction
2.Parallel LCD Construction and Testing
3.WinAmp Installation and initial testing
4.Initial WinAmp and LCD implementation testing

1.Socket 7 System Construction

The socket 7 system began as a used AT computer case and motherboard. These parts
were per cured from an auction sale at Old Dominion
University for $5.00. The system also came with a 250watt
power supply, floppy drive, Yamaha Soundcard, and CD-
Rom. A 730 MB hard drive, 32 MB RAM, and a Pentium
166 MMX were installed to complete the unit.

Upon initial startup it was found that the motherboard had a
bad CMOS battery. Although this is not a major issue
normally, this issue was sure to delay startup when a monitor was not connected in future
stages. It was also found that the CD-Rom drive, which came with the case was bad. The
drive would try to read CD media but could never mount the directory. The Office of


Naval Research at Elizabeth City State University solved this problem with the donation
of a 24X used CD-Rom. Once the replacement CD-Rom was installed, operating system
installation could begin.

Windows 98se was used as a base operating system due to the fact that per the system
specifications, this operating system would run WinAmp the best. The installation of the
operating system went relatively smoothly. The
only driver that had to be installed after the
operating system was for the sound card, which
was a simple download. The installation of
WinAmp also went smoothly. Samples of ten
music MP3 files were also installed for testing of
WinAmp sound quality. Once the system had been “burned-in” construction on the
parallel LCD began.

2.LCD Construction

The actual construction and design of the HD44780 LCD parallel interface was by far
one of the most hands – on components of the entire project. This portion of the project
actually began with research in to the workings of the HD44780. Soon it was found that
this LCD was often modified for use in computers to display related system information
(i.e., temperature, network traffic, hard drive space, etc..). One website in particular gave
not only a wiring schematic but also pictures and software examples


(http://www.overclockers.com.au/techstuff/a_diy_lcd/). While researching this it was
discoverd the LCD requires two 5v sources, one to power the backlight, and the other to
power the LCD itself. Many websites offered ways of rewiring the 2.5v connection of a
standard parallel to “Jury rig” the power. It was decided there had to be a better way
through the use of the 5v output of a standard USB (universal serial bus) port. Modifying
a USB cable to strip out the data only left the 5v connection. This was a straightforward
solution to an electrically complex problem.

Construction began by first de-soldering the HD44780 from the control module board
from which it was originally attached. Once removed a standard DB-25 to Centronics
Parallel cable was taken apart. Both items were previously acquired before the beginning

```
Drawing Power From Printer Port
```
Resisters are used to control the flow of power as well as, multiple extra connections.
With the use of direct power, these resisters are removed.
Provided by: [http://www.myrolypoly.com/lcd_project/lcd_project.html](http://www.myrolypoly.com/lcd_project/lcd_project.html)


of this project though, street prices for the HD44780 range from $10.00 to $30.00. The
parallel cable can range from $5.00 to
$25.00. The wires on the parallel cable
were numbered during production. The key
wires were each with a volt-ohm meter to
make sure there were no connection
problems. Once all wires had been tested
successfully. The data wires, USB power wires, and
connection points were pre-stripped and pre-soldered. The following guide was then used
to connect all data and power wires:

```
LCD pin Connect to Function
1 Earth (Black wire on USB connector) Earth
2 +5V (Red wire on USB connector) Power
3 Earth (Black wire on USB connector) This adjusts the contrast of the LCD digits. Earthing^
pin 3 provides maximum contrast. A 10k pot can be
4 Parallel Port pin 16 (Green/white wire) Register Select
5 Earth (Black wire on USB connector) Read/Write. Since we are not going to read data from^
the LCD, we can ground pin 5; to set it permanently in
6 Parallel Port pin 1 (Pink wire) Enable - Strobe
7 Parallel Port pin 2 (Red wire) Data bit 0
8 Parallel Port pin 3 (Yellow wire) Data bit 1
9 Parallel Port pin 4 (Green wire) Data bit 2
10 Parallel Port pin 5 (White wire) Data bit 3
11 Parallel Port pin 6 (Blue wire) Data bit 4
12 Parallel Port pin 7 (Purple wire) Data bit 5
13 Parallel Port pin 8 (Pink wire) Data bit 6
14 Parallel Port pin 9 (Grey wire) Data bit 7
Bl-P +5V (Red wire on USB connector) Backlight +5V
```

Bl-N Earth (Black wire on USB connector Backlight Earth

```
Once all the wires were soldered on, the LCD was connected to the socket 7 based
computer system, which had been previously constructed. There was one minor problem
in connecting the modified USB to the computer, the
socket 7 architecture pre-dated USB ports. To remedy this
situation a $15.00 PCI to USB card was installed in the
system. The drivers for this card were already preinstalled
in Windows 98se though the drivers were not necessary to
only draw power from the port. Lastly the LCD was
connected to the parallel and USB ports on the host
computer system and a test signal was received showing that
all connections were in good and working order. To protect
the wires from strain they were incased in non-conductive
hardening silicone. The wires were also put in a double layer
of heat shrink tubing to protect them. These two additional
preventative measures would allow a certain ruggedness,
which would be, needed in future steps. Temporarily the
LCD was installed in a cardboard box until a suitable case
was to be used in Stage two for the custom controller.
```
```
3.WinAmp Installation and initial testing
```

WinAmp version 2 was used as opposed to the most recent version three due to the
overwhelming amount of support and information on the older version. During the
installation WinAmp automatically linked itself to all supported media types (i.e., MP3,
WAV, CDDA...). After installation was completed keyboard direct commands were
found. Fortunately the keyboard commands were built into WinAmp without the need for
a plug-in or skin.
Special note was taken of the
Play, Pause, Next Track, and
Previous Track keyboard
commands. These commands
would be necessary to use
WinAmp in future stages
without the use of a monitor or
mouse. These keyboard
commands would also be hard

wired into the custom controller for Stage 2. While using
WinAmp with the sample files previously copied, the Yamaha Sound Card was found to
be very much inferior. Clicks, Pops, and a high Pitch hisses often accompanied all music.
Considering the fact that a car alternator could throw even more noise into any playing of

*** Main Window Keyboard Shortcuts ***
Key---------------------------------------------------------------------------- Action
--
(Options/toggles)R Toggle Repeat
S Toggle Shuffle
(Playback controls)X or Keypad 5 Play/Restart/Unpause

V Shift+V StopStop with Fadeout (^)
Ctrl+VC Stop after current trackPause/Unpause
B or Keypad 6Z or Keypad 4 Next TrackPrevious Track (^)
Keypad 1Keypad 3 Jump Ten Songs BackJump Ten Songs Forward (^)
Left Arrow or Keypad 7Keypad 9 or Right Arrow RewFast-forward 5 secondsind 5 seconds (^)
(^) L or Keypad 0 Open/Play File
Ctrl+L or Ctrl+Keypad 0Shift+L or Insert Open/Play locationOpen/Play Directory (^)
Keypad 8 or Up ArrowDown Arrow or Keypad 2 Turn Volume UpTurn Volume Down (^)


a track, a different soundcard in future stages of the project would be used.

4. Initial WinAmp and LCD implementation testing

The final objective of Stage one was to display MP3 information from Id Tags in
WinAmp to the parallel LCD. Original research found that LCD drivers are actually built
into WinAmp. During actual it was found that this research was slightly flawed. The
LCD drivers are only in WinAmp 3, and a specific wiring configuration had to be used
for correct operation. This was not a feasible solution so once again information was
found at the Overclockers web site about a pre-programmed solution. The solution cam in
the form of a program called LCD Center 2.0. This program was written to not only
display information from WinAmp, but also displayed system information. To put it
simply it seamed to be an all-in-one fix. There is a proverb in the bible that all that
glitters is not gold and this was so in this case.

Though LCD Center 2.0 loaded fine, no display showed on the LCD. After much
research and reconfiguration, it was found that in order to use LCD Center, a third
program had to be installed to translate software-based serial requests, to hardware-based
parallel requests. This program was called DriverLINX Port I/O Driver. Upon installation
of this program the LCD displayed it’s first text, which was a generic screen that said
“Thank You For Using LCD Center 2.0.” Upon this success WinAmp was opened and
played an MP3. The MP3 file Id information was successfully displayed, however; it was


noticed that after a period of about five minutes the LCD would always lock. From this it
was decided that a different LCD Driver or WinAmp plug-in would have to be found as
the LCD was to be the main display for future stages.

In preparation for stage two settings were experimented using WinAmp as the default
shell as to not allow any other programs to interfere with MP3 play. Unfortunately it was
discovered that in order for a program to be used as a shell, it could not use any other
functions of other programs. Due to this the original plan to create a shell was altered and
it was decided to use a menuing system. To test future processes LCD Center 2.0,
DriverLINX, and WinAmp were set as startup programs in the startup group of windows.
These allowed the computer to successfully startup without a monitor and automatically
began playing MP3s with the parallel LCD as the primary display. The one problem
noticed was that from power-on to actual MP3 music took approximately 5 minutes. In
driving terms, a driver would go five miles before the system could be used. A solution to
this problem had to be found in Stage two for actual road trials.

Stage 1 Conclusions:

WinAmp was found to have built in Keyboard Commands that can be used in the custom
controller. A different parallel LCD driver had to be found to increase reliability
otherwise while in road tests; understanding of what the computer was doing would be
lost. The system booted extremely slowly. Either an alternative Operating System or
Computer System had to be used for future testing.


## Stage 2

Objectives:

1. Implement Power Inverter
2. Use computer from within vehicle with Cassette to Phono Adapter
3. Find a better LCD Driver
4. Construct Custom Controller
5. Implement operating system modifications to speed boot time.
6. Implement device to cancel line noise from computer.
1. Implement Power Inverter

During preliminary research into ways to power a computer from within a car one main
fact arose time after time; the power inverter had to
have more wattage than needed otherwise the inverter
could heat up and fail. The final design called for a
~150watt mini ATX power supply for the main
computer along with any TFT LCD power considerations. This meant at minimum a
~200watt power inverter would be needed. After weeks of searching stores and Ebay, a


small company that sold 400watt power supply’s for $27.00 was found as opposed to the
standard $50.00 for a ~300watt power supply. The power inverter had a cooling fan in a
heat-sink style case, which means very low temperatures. It came with dual ~120VAC
outlets to allow multiple AC devices to be connected. The power supply also has an
alarm and automatic shutoff in case of sub 10VDC from the car. The power inverter was
tested in the vehicle using an old black and white TV, which worked perfectly.

2. Use computer from within vehicle with Cassette to Phono Adapter

With the arrival of the power inverter there were no
longer any reasons to not connect the computer up in the
vehicle. The case of the computer was positioned of the
in front of the passenger seat to prevent damage during
initial travel. To use the car speakers a cassette to Phono
adapter was connected between the stock car radio and
output jack in the computer’s sound card. A standard AT keyboard and the LCD was also
used in the initial trial run of the Carputer. Though the computer powered on, the
previous stages problem of a slow boot truly came to bear because there was no monitor
to watch. It was uncertain if the system was correctly booting or not. After approximately
five minutes the “Thank you for using LCD Center 2.0” message appeared and WinAmp
began to play its first song from with in the vehicle. The car alternator did not inhibit the
sound quality of the music but the same sound faults from stage one were still noticeable.
As the song began to play a few WinAmp keyboard commands were used to make sure it


was responding. Everything tested fine so then the car out was taken out for a drive.
Immediately it was noticed that when any series of
bumps were hit in the road, the music skipped. It
was not know if the problem was with the hard
drive not being able to take the shock of road travel
or if the limited amount of system memory could
not allow the creation of a sufficient buffer. Once
the first test was completed it was noticed that the
LCD driver had locked as it had done in stage one testing. These initial findings though
exciting were also cause to find further solutions to make the system function better.

3. Find a better LCD Driver

With the constant failures of LCD Center 2.0 a search for an alternative way to control
the parallel LCD began. The idea that WinAmp 3 had LCD drivers’ built-in was first
explored. The Internet was searched for a WinAmp 2 plug-in that could do the same thing
as LCD Center 2.0, but was also suited to the wiring configuration already used.

After much searching a plug-in called “ Winamp OpenSource LCD Plugin for various
LCD & VFD modules (http://www.markuszehnder.ch/projects/lcdplugin/)” was found.
This plug-in not only stopped the lock-ups of LCD Center 2.0, but also gave the added


bonus of working directly in WinAmp as opposed to being a third-party piece of
software, which had to also run in the system background.

4. Construct Custom Controller

During the initial testing phase a standard keyboard was used to control WinAmp through
keyboard commands. To reach from the steering wheel to attempt to push one key on a
104 button keyboard with a mere glance is
nearly impossible and is definitely unsafe. To
make use of the keyboard commands easier,
momentary push buttons were hard wired to the
keyboard controller. The most difficult portion
of this construction was the tracing of the
keyboard circuitry back to the main control board.

The keyboard itself was composed of two plastic sheets. These sheets had electrodes
which when a button was pushed would create a certain connection which would produce
an ASCII code. This code was then
interpreted as a particular character. It was
decided to hardwire the Numpad numbers:
5(Play/Pause), 6(Fast Forward/Next Track),
and 4(Rewind/Previous Track). First a
marker was used to mark the track of the


connection to the main circuit board. After tracing the connections a volt-ohm meter was
used to make sure the connections were correct when each button was pressed. Next
wires were soldered for each button; fortunately all three buttons used the same ground so
only four total wires were needed. Once the wires were soldered the momentary push
buttons were mounted in a plastic kit case and tested. Both the hard-wired buttons and
keyboard keys functioned perfectly. To complete the custom controller the parallel LCD
was installed into the plastic case and also a power button and a power LED were hard
wired into the case. A standard RJ-14 modular telephone cable and jack were used to add
connections to the computer case while allowing the ability to easy disconnect the custom
controller from the computer system.

Road testing of the custom controller was most definitely a better experience than the
previous one controlled by keyboard only. The buttons were positioned in such a way as
to give the user the ability to feel the buttons and to select the needed function allowing
them to not have to take their eyes off the road. The custom controller not only made the
Carputer more user friendly, but also safer for the driver to use during travel.

5. Implement operating system modifications to speed boot time.

As previously stated the Carputer had one major flaw, boot time. Five minutes for a
computer to boot is not feasible in any system much less one in a vehicle. It was decided
to abandon the Socket 7 architecture and to look for a more powerful machine. Thanks
once again to The Office of Naval Research; a Pentium III 400mhz machine was donated.


This machine was two generations above the original Pentium 166 used. Thanks also to
the donation of a co-worker Kurt Baker, the Carputer boasted
128mb of RAM as compared to the previous 32mb. To add
additional storage a PCI SCSI (Small Computer Standard
Interface) controller and 2G hard drive were installed. Because
the new system had USB ports on the motherboard, the PCI to
USB controller was no longer necessary.

Once Windows 98se and WinAmp with LCD Plug-in were installed, the differences
between the two systems were immediately prevalent. To begin the boot time dropped
from five minutes to under one minute. This was a vast improvement over the previous
system. It was also found that due to the greater amount of RAM, full music files could
be loaded in memory. This completely removed skips in the music due to rough driving
conditions. The change of systems also solved the CMOS battery problem that would
often reset all data on the original system. The only residual problem from the previous
system was that of sound quality.

6. Implement device to cancel static noise from computer.

First this problem was tackled by looking into the purchase of a line filter until the
systems change and the same problem connecting to regular computer speakers
continued, outside the vehicle. It was decided to replace the sound card before investing
$30.00 into a line filter. The Yamaha soundcard was removed and a Creative Sound


Blaster 16 was installed. The clicks, pops, and hisses immediately went away leave a
clean rich sound. T the computer was then tested in the vehicle and the clean, rich sound
remained. The fault was in the original sound card itself. The true proof of this would be
in future steps when the new motherboard with sound would be tested.

Stage 2 Conclusions:

All of the concerns from stage one were addressed and solved. To say the least when
building an in car computer, skimping on the technology for economical reasons caused
more problems than they solved. The custom controller is an absolute necessity, even
when future Stages have a full Color TFT LCD, the custom controller allows the driver to
easy and safely use the Carputer during travel. The standard hard drives showed little
signs of wear during travel and would therefore be used in future stages. WinAmp plug-
ins worked much better than third party software and did not lock up.

## Stage 3

## Objectives:

1. TFT LCD Implementation
2. Socket 370 Motherboard installation and testing
3. Carputer Menuing system


### TFT LCD Implementation

The TFT LCD would allow the Carputer to perform all the functions a normal computer
while both conserving space and power. The decided
LCD to be used was that of a Playstation One mobile
gaming console. The viewable size of the LCD was only
five inches, which was equivalent to a standard car LCD
screen without the associated price. During initial
research it was found that the LCD could be modified to plug into a standard SVGA port
on a video card. The one draw back of this design was the fact that the modification
would permanently make the LCD a computer monitor.

Once the LCD was purchased an immediate change in the
design of the Carputer had to be addressed. The
connectors, which had to be soldered, were microscopic
in the newer versions of the LCD screen. The alternate
plan was to use the "A/V In (Audio/Video In)" port on
the LCD to input composite video from the computer.
This change meant the video card from the Carputer would need to have composite
video-out capability. This also meant a cable would have to be modified to accept the
composite video-in through a RCA type connector. The A/V cable required a special
four-input 1/4" Phono connector to plug directly in to the Playstation LCD. These
connectors allowed a video, right channel, left channel, and a shared ground to be


transmitted to the LCD. The standard A/V cable was ordered separately to connect to the
Playstation LCD. Upon arrival the cable was modified from its standard dual 1/4" Phono
ends to a single 1/4" Phono and three RCA connectors. The left channel, right channel,
video, and grounds were all separated out into their individual wires and soldered to a
standard RCA connection of left channel, right channel, and composite video.

Connecting the composite video and sound cables to the output of a standard VCR tested
the LCD. It was found that the LCD only activated when a signal was present otherwise
the LCD remained off. The picture clarity on the LCD was also superb. This was a main
concern because this would soon become the main way to control the Carputer.

### Socket 370 Motherboard Installation and Testing

The original design of the Carputer included the use of a newer motherboard and
processor, which could handle the demands of all the features in the Carputer. The
original designed called for a very inexpensive motherboard and processor with video
onboard. Due to the design changes in the connection between the LCD and video signal,
a different type of video-out would be needed either on the motherboard or video card
purchased for the Carputer. It was decided to Purchase the VIA EPIA 800 All In One
Motherboard that would solve all the problems with the new design of the LCD and also
had the perk of an extremely small footprint.

### VIA EPIA Mainboard Specification (Provided by: VIA Technologies)


Standardized Embedded Solutions for Total Mainboard Connectivity
Form Factor - Mini-ITX

- 170mm x 170mm- Micro ATX Chassis Compliant (^)

- VIA C3™ E-Series processor (EBGA
package)
- 100/133MHz Front Side Bus

- 128K L1 and 64K L2 cache Chipset - VIA Apollo PLE133 (^)

- VT8601A North Bridge
- Featuring integrated AGP 4X graphics
- VIA VT8231 South Bridge
TV- S-Video or Composite video output-Out - High quality scaling and filtering
- Supports NTSC/PAL TV formats
Main Memory - Two 168-pin DIMM

memory- PC100/133 SDRAM support sockets (^)
LAN - VIA 10/100 Ethernet LAN onboard
Graphics - Integrated AGP4X with 2D/3D Graphics Acceleration

- Motion Compensation for DVD playback

Audio - 3 Audio Jacks - VIA VT1612A AC'97 onboard- Line-Out, Line-In and Microphone (^) -In

- Sound Blaster, Sound Blaster Pro Compatible
- Digital I/O compatible with consumer mode S/PDIF
Expansion Slots - 1 PCI slot

Onboard IDE I/O Ports - 3 Audio Jacks - ATA/100/66 - Line (^) -out, Mic-in and Line-in

- Four USB ports (two USB ports located at rear side)
- 1 EPP/ECP parallel port
- 1 16C550 compatible serial port

- 2 External PS/2 Compatible Key- 2 TV output ports (S-Video or optional RCA TV out)board /Mouse ports (^)

- 1 S/PDIF out (optional and multiplex with RCA TV out)
- 1 RJ-45 LAN port
- 1 PCI slot (Note: support for two PCI devices)
Power Supply -ATX Power Supply Compliant


Once the motherboard was received a couple jumper changes had to be made to allow the
video to display through the composite video jack. Once the changes where made the
motherboard was mounted into a test system with and ATX power supply. The hard drive
was also upgraded to a Maxtor 10GB drive to
allow space for the operating system, DIVX
movie files, and mp3 music files. A Hauppauge
Win TV PCI video card was also added to the
Carputer. The operating system was upgrade to
Windows XP Professional to give the Carputer
greater software stability and upgrade-ability. An
USB Thumb mouse was added to allow the on-screen cursor to be easily used. The
original parallel LCD was lastly connected and tested fine with the new operating system
and motherboard. The whole unit was then reinstalled into the vehicle.

Initial testing in the vehicle was very cumbersome. Use of the Carputer was nearly
impossible while driving due to the small size of the screen and icons. Some issues were
overcome by changing the screen appearance to a "High Contrast" setting. Other visual
options that aided control of the operating system was to increase the size of the icon as
well as remove any unnecessary icons from the desktop. Thought these options increased
the feasibility of the Carputer, a larger menu driven program would be necessary to tie all
features of the Carputer together.


### Carputer Menuing System

The success or failure of the Carputer hinged on the ability for the Carputer to be driver
friendly. This "friendliness" is solely the responsibility of the GUI interface or menuing
system. Initial research found that a Windows shell or flash-based menu program would
be the best solution to this problem. Initial research also found that either voice control
and/or a touch-screen would add to the experience of the user. Unfortunately due to cost
limitations, a touch screen was not possible but a voice control system seamed very
feasible. Windows XP Plus had an add-on feature for Windows Media Player, which
would allow voice command control. This option seemed the logical solution to complete
the Carputer project.

The voice command installation began by first installing the most recent version of
Windows Media Player. Upon initial test of Media Player it was found that the parallel-
based LCD was not compatible however the use of the main LCD and voice commands
would make it irrelevant to the project if the voice command worked properly. The play
list features were also very difficult to control, but all needed media formats played
without a problem. Media Player also had the added feature of displaying visualizations
during the playing of music files or CDs. Windows XP Plus Media Edition was then
installed with the option to include Media Player Voice Command turned on. A
"Gooseneck" microphone was also added to the system to accept the voice commands.


Initial testing was promising. Voice commands worked flawlessly until it was discovered
that any music or movie being played would cause the computer to do many unwanted
tasks. Things from creating new playlists, to skipping songs, to deleting song would
occur if a clear song were played in the vehicle. One other problem with the voice
command was the lethargic nature of the actual commands. Saying "DJ Next" to get to
the desired track in a 500-song database would often become frustrating. This form of
control was deemed unfeasible and a better menuing system was once again considered.

It was found that Windows XP Profession had a new version perfectly suited to the needs
of the Carputer. This newer version was called Windows XP Media Center Edition.
Many Internet sources claimed Media Center was simply an add-on shell for Windows
XP. Unfortunately this was proved to be incorrect. Although Windows XP Media Center
Edition was built on the Windows XP base, Media Center Edition required specific
hardware, and could not be reconfigured to suit the Carputer. During the research phase
of this problem other menu driven shells were discovered such as “Couch-Click”,
“Showshifter”, and “Media Engine.” The programs Couch-Click and Showshifer were
both major disappointments in that user control was very difficult. Media Engine on the
other hand had been designed for car-based computers and allowed seamless access to all
functions of the Carputer by the driver while also allowing customizability for other
upgrades.

Media Engine is a user interface to be installed on a Microsoft Windows based PC in an
automobile. It features a media file player based from Windows Media Player 9 that uses


an internal Microsoft Access database to organize media within the program
(http://www.mediaengine.org/index.php?FAQ).

### Stage 3 Conclusions

The inclusion of a Color TFT LCD took the Carputer to a whole new level, and with that
level came many new answered and unanswered problems. The LCD modification
change called for a new type of video output to the screen. In trying to find a video card
that would suit these needs and new motherboard was decided upon. This fundamental
change brought about the possibility of making the Carputer mobile. This is a question
that would be explored in the final stage. The addition of the color TFT also brought a
problem of control. Through research a viable menuing program was found, however the
change to the menuing system alleviated the use of a custom controller and a focus on
mouse control. This change made the use of the Carputer unsafe for a driver. The only
true way to completely solve this problem would be the addition of a touch-screen.
Unfortunately budget constrictions would not allow this addition. Though the Carputer
was fully functional the question of feasibility started to control the focus of the project.

## Stage 4:

### Objectives:

1. Custom Case Construction
2. Direct Audio Implementation


### Custom Case Construction

During the initial research into the implementation of the Carputer it was decided that a
full-scale dash installation and modification would be one of the final steps of the project.
It was found that there would be severe size limitations in the installation but the over all
effect would give the Carputer more of a custom look and feel. Though this sounded like
and excellent idea other factors soon changed these initial findings. One major decision
was that the Carputer should be portable. This decision came about during a major
hurricane. During travel back and forth, it was decided that a functional, mobile Carputer
would allow any vehicle to have the capability of entertainment or news when wanted.
Do to this fact the initial dash installation was scrapped and new portable case designs
were considered.

During the redesign process three main types of cases were debated, a speaker case
installation, a vehicle trunk installation, and a tool case installation. Initial speaker case
designs had to be dismissed due to the fact that a speaker case would not protect against
interference and a speaker case would not be ideal to keep a steady airflow to prevent
overheating. The second design to install a standard case into the trunk of the vehicle
called for the use of extremely long cables to run from the back of the vehicle to the
front. This design would have also made the user stop the vehicle and get out to insert a
CD or DVD into the Carputer. The third design called for the use of a standard plastic
toolbox. This toolbox would allow the Carputer to have a small footprint, made the
Carputer very portable, and the case itself was water tight to protect the inner electronics.
This idea by far seemed the most logical of the three case designs.


The tool case design started with the laying out of all the components. The actual case
decided upon was just large enough to allow the Mini-ITX motherboard to lay flush on
the bottom. The other components were the dry fitted including the power supply, hard
drive, CD Rom, and TV Card. While fitting the PCI TV Card it was found that the case
did not have enough vertical space to insert the card. It was decided that the TV card was
not a major portion of the Carputer final design so it was removed. In order to connect to
the different ports on the Carputer access ports had to be added to the case.

The modification of the case began with the
installation of the Motherboard plate. This plate
allowed access to all the ports on the
motherboard while only cutting a single
rectangle into the side of the case. The plate
actually contained machine pressed wholes for
the PS/2 ports, USB ports, serial port, video
ports, and parallel port. Once this whole had been cut using a Dremel tool, the plate and
motherboard were inserted to mark the mounting positions for fasteners to be installed.
The marked spots were drilled and standard brass standoffs were installed. The
motherboard was then mounted using screws in the standoffs.


A whole for the 200-watt power supply
was then cut into the back of the case. The
power supply was a small ATX power
supply from an older computer. During
this installation it was decided to increase
airflow to the case by moving the power
supply fan from in the power supply to the
top of the case. Cutting and lengthening the connecting power wires to the fan of the
power supply accomplished this. The metal case was removed from the power supple to
allow the air to flow around the heat sinks with in the power supply. The modified power
supply was then mounted to the back
of the case and attached with screws.
The fan would be mounted to the top
of the case once all other components
had been installed.

When the Carputer was being both
researched and tested, it was found that it is best to mount the hard drive perpendicular to
the ground to prevent data loss due to bumps in the road. This idea was taken one step
further by adding a shock absorber to the sides of the hard drive. The shock absorber used
was a piece of a Temperpedic Bed generously donated by Temperpedic. This space age
material formed a glove of cushion around the drive. The material was attached with two
metal plates which and log screws not fully tightened. This allowed the Temperpedic


material to absorb any shocks, not the drive itself. The hard drive and shock absorber
was then mounted into the case. The CD Rom then became the last major component that
had to be mounted.

First, a whole was cut into the side of the case to
allow the CD Rom to be inserted. A wooden frame
of sorts had to then be installed to keep the sides of
the case stiff, hold the CD Rom flush, and secure
the CD Rom in the case. Two metal plates were
then attached to the sides of the CD Rom and were screwed in the wooden framework.
Once this had been completed a fan whole
was measured and cut in the top of the case
for the fan from the power supply. All wires
were then run and a power switch and the fan
were mounted. This ended the physical
construction of the tool case and left only
testing to be done.

Upon booting the Carputer all systems powered up and worked without a hitch. The
temperature within of the case remained within the limits of the motherboard and
processor. The Carputer was left overnight to run a burn-in program, which found no
problems.


### Direct Audio Implementation

With the decision to make the Carputer portable some changes had to be made to the way
sound would be outputted to the vehicles sound system. During the research stage of the
Carputer a trip to Go-Ho AutoAudio in Virginia Beach, Virginia was taken. An Audio
Consultant named Casey Jones aided the project by giving some advise on how to
connect any device to speakers. From this meeting the need of ground loop isolators and
amplifiers was taken. Unfortunately this information would not help in the new design
structure, however a “backup plan” was also discussed. The uses of a RF stereo sending
unit or a radio with an auxiliary channel were considered. An RF sending unit would
allow the Carputer to transmit any audio signal to a designated radio station on the
vehicle. This would allow the Carputer to transmit to any standard radio tuner and would
also remove the need for wires to be run. The option of using a radio with an auxiliary
input would allow better sound quality however this option would make the Carputer
vehicle dependant. This meant the RF Sending unit would be the best decision to
complete the Carputer project. Unfortunately a good stereo RF Sending unit would cost
approximately $100.00, which the budget of the Carputer would not allow. It was decided
the Stereo Phono to tape converter would continue to be used.

### Stage 4 Conclusions:

The decision to make the Carputer Portable greatly affected this stage of the Carputer.
The modifications of the toolbox case not only made the Carputer portable but also safer
in that a potential burglar would see the case and think nothing of it, as opposed to a
computer case and know exactly what he/she would be getting. The case also allowed the


installation of a slotted CD-Rom to more accurately simulate a standard car CD player.
The audio implementation on the other hand had both perks and disappointments. The RF
Sending unit would be a great additional to the Carputer in future upgrades however until
such time the original device used to connect the Carputer to the tape deck would still be
used. Over all this stage was a success though it turned out completely different from the
original planning stage designs.

## Project Conclusion and Future Expansions

### Functional by not Feasible

Initially the Carputer’s purpose was to detail the conception, design, and implementation
of a computer into a stock 1998 Dodge Neon vehicle. Though this was done the changes
that occurred along that way deviated from the initial design by leaps and bounds. Most
of the changes occurred due to portability, safety and use issues. A five inch active TFT
LCD from a Playstation does not have the resolution needed to view text of normal 12 to
14 pitch font. Items on the desktop or in a program were often hard for the user to
identify. Though some of these limitations were over come with the use of large fonts and
icon sizes, all programs did not have such schemes for the visually limited. Accessibility
options in Windows made many applications conform, but not all. One example of this
limitation was the fact that the Carputer had access to the Internet through a cellular
phone but could not be used due to the poor picture quality. When the active LCD was
added a little know law in Virginia almost stopped testing of the Carputer all together.
The law stated that the only video display screens that is allowed to be display in front of


a driver had to either be used for GPS (Global Positioning System), or a rear camera for
backing up. In North Carolina this was not an issue so testing continued.

Use of the Carputer once again almost came to a stop because of the graphical user
interface. Using a computer while sitting in front of it with a mouse is fairly simple, but
use while driving became dangerous until the menuing system was implemented however
this did not fully solve the problem. To make the system a fully feasible product both a
larger screen and touch sensor need to be added.

Portability made the Carputer more feasible by taking away vehicle dependency. The
addition of a RF Sending unit would allow the Carputer to fully function in any vehicle
through a standard radio tuner, while the tool case design could allow the Carputer to be
stored easily in any type vehicle. The portability factor also added to the functionality of
the Carputer by allowing the unit to be used as a Lan Party machine (a computer used on
a network for video games.) This expands the use of the Carputer but starts to lean into
the realm of the Laptop.

### Carputer vs. Laptops

Though Carputer performs all the functions a traditional laptop could perform, it has a
few distinctively beneficial qualities that set it apart. First and foremost the Carputer costs
about a third less than a comparable laptop. A laptop is constructed using many
proprietary components. These components though smaller, cost the manufacturer much


more to produce, there by increasing the cost of a laptop. A similarly equipped laptop
costs between $799.00 and $1200.00 depending on the brand selected. The Carputer in its
present form cost a grand total of $345.00 including the estimated costs of donated
components.

The Carputer also has the great benefit of being able to use standard replacement
components as opposed to brand dependant laptop components. One example of this is if
the 10 GB hard drive went bad in the Carputer ~$50.00 could be spent to purchase a 20
GB replacement. In the laptop world a 20 GB hard drive cost ~$170.00 depending upon
where it is purchased.

Laptops do have the ability to function on battery power where as the Carputer needs
direct power from either a power inverter or outlet but even that function can be
dismissed as there are laptop companies that now do not provide batteries with the stock
units. For this and previously discussed reasons the Carputer is for a different type user
than a normal laptop user would be.

### Carputer Uses

The Carputer was designed for two types of users, those who like modified vehicle
designs and those who need the convenience of a home computer with out the cost of a
laptop. One example of the initial type of user is a racecar driver who would like to view
real-time stats on vehicle performance and even do an on the fly tune-up. The same type


of user may have kids or a bus full of pit crew who ride with him/her to different events
around the country in which the Carputer could be used for entertainment or for GPS
travel.

The second type of user could be businessperson whose vehicle is a mobile office. One
type of businessperson could be an auto adjuster who could take photos of a damaged
vehicle, pull-up a person’s policy and cut the person a printed check while sitting at the
location of the accident. Another type of business user could be a truck driver who uses
the Carputer to keep track of mileage or freight while taking the Carputer into the back of
his/her cab during a break to watch a movie or check email. With a wireless broadband
link the trucker could even videoconference a call home to check on his/her family while
on the road.

### Future Expansions

The first recommended expansion of this Carputer is the addition of a 7” TFT Touch
screen from Xenarc Technologies. This screen actually uses a SVGA connection and was
tested above 1024 X 768 screen resolution without picture loss. The addition of the
touch-screen would also add a greater feasibility factor to the unit. This screen was priced
at $499.00 from Xenarc’s website at the time of this project but as all computer product
prices, the price will drop with time. A GPS Receiver and software would also be a great
addition to the Carputer. At the time of this project a Delorme Earthmate USB GPS
Receiver cost $124.00 with Street Atlas software included. To aide in the delivery of


content from a home network the addition of a wireless network card would make the
transferring of Divx movies or MP3 sound files very easy. To turn the computer on
remotely a 12 volt remote controlled relay could be added to turn the unit on or off with
out leaving the comfort of a users home. Because of the limitless expansion possibilities
of the Carputer the future of the Carputer could change as the users needs change but the
greatest addition would give the Carputer the ability to be used as a pocket pc could be
used. The OS could be embedded into a chip on the motherboard so a fast boot time and
shutdown time could allow the Carputer to take control over all the functions of a car
such as climate control, engine monitoring, anti-theft system, and possibly with the future
development of technology a type of auto-pilot for a vehicle. The future is a bright one
for the designer who takes the Carputer that extra step to make it a must for any future car
owner.


## Acknowledgements:

Sonya J. Powell
Mary B. Powell
Professor Kristna Kulkarni
Dr. Linda Hayden
Joal Hathaway
Dr. Carol Jones
Kurt Baker
Keith Martin
Robert Hunter
Casey Jones
MazdaPC & ZPC Headquarters
Go-Ho Auto Audio in Virginia Beach, Virginia
B & B Auto Parts and Crushing, Inc.
MP3 Car
Office of Naval Research Lab at ECSU
Aviation Lab at ECSU
Old Dominion University
Tech Buys
Radio Shack in Franklin, Virginia


