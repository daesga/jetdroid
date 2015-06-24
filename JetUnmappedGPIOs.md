# Introduction #

The JetDroid project has made some good progress in the past. In order to ensure we can continue at this pace and make good progress in the future I am now asking you for help. What is needed is some missing information about the Jet hardware. Knowledge of this is essential for further development and driver support for all parts of the phone hardware. Without this information support for some parts of the hardware cannot be developed (at a reasonable effort)

# How can you help? #
If you know someone who has access to Samsung schematic diagrams please ask if you can get the missing information or take a photo of parts of the schematics. I know that it is most probably impossible to get a copy (e.g. PDF) of the schematics, thus I am just asking for some information. So, if you best friend is working in a phone repair shop and he or she as access to this kind of information, please ask this person.

**If you don't have this information or know someone who has it please don't write to Samsung directly. This was tried before and will not help. You can still help by spreading this request to other forums or to other people who could know other preople who know.**

# What is needed? #
To fully understand the phone hardware we need to know to which port e.g. of the main phone processor the peripheral chips (e.g. WLAN, bluetooth, modem, sensors, etc.) connect to. All pins/ports of the processor have names and we know them. What we need to know is to which signal (names) these pins connect to. In some cases the connection to the main processor (S3C6410) is known but it is not known where the other end is connected to.

# How to provide this information? #
Below I have compiled 4 lists. List A lists pin names of the phones main processor S3C6410 (in the schematic diagrams it is referenced as UPC701). If you can help please provide connections like e.g. XM0ADDR12 -> LCD\_SCLK (which means pin XM0ADDR12 connects to signal LCD\_SCLK). Completing this list is of highest performance

List B list signals of which the name is known but it is not known where on UPC701 they connect to. Please provide connection information like for pin A. All signals on this list should connect (at least) to one pin from list A

List C lists signals of which the name is know as well as the connection to UPC701. For these signals the other end of the connection is needed. Please specify connects like BT\_HOST\_WAKE -> U201 (BT\_GPIO\_1) which means signal BT\_HOST\_WAKE connects to pin BT\_GPIO\_1 of U201. For this list only connections to components other than UPC701 are needed.

List D lists signals of which the name is know but it is not know where they connects. For these signals information like for list C are need but the do not necessarily connect to the main processor UPC701

= Too complicated?
If you have access to the required information but don't know how to read the schematic diagrams, please search for as many of the names below and shoot photos for the different sections of the schematic diagram pm me or mail them to dopi711 (at) googlemail.com.

I hope you can help to resolve the missing connections.

Cheers,

Dopi

# The 4 lists #
Below are the 4 lists mention above. The number of open pins / signals can give you an impression of the amount of information that is need for successful continuation of the JetDroid project.

## List A ##
(Pins of UPC701 (S3C6410) for which the name of the connecting signal name is unknown, please provide signal name)
  * XHIDATA6
  * XHIDATA7
  * XHIDATA11
  * XHIDATA12
  * XHIDATA13
  * XHIDATA14
  * XHIDATA15
  * XHIDATA16
  * XHIDATA17
  * XHICSN
  * XHICSN\_MAIN
  * XHIOEN
  * XHIINTR
  * XEINT0
  * XEINT1
  * XEINT2
  * XEINT3
  * XEINT4
  * XEINT5
  * XEINT6
  * XEINT7
  * XEINT8
  * XEINT9
  * XEINT10
  * XEINT11
  * XEINT12
  * XEINT13
  * XEINT14
  * XEINT15
  * Xm0OEata
  * XURXD0
  * XUTXD0
  * XUCTSN0
  * XURTSN0
  * XURXD2
  * XUTXD2
  * XURXD3
  * XUTXD3
  * XIRSDBW
  * XSPIMISO0
  * XSPICLK0
  * XSPIMOSI0
  * XSPICS0
  * XSPIMISO1
  * XSPICLK1
  * XSPIMOSI1
  * XSPICS1
  * XPCMEXTCLK0
  * XPCMDCLK1
  * XPCMEXTCLK1
  * XPCMFSYNC1
  * XPCMSIN1
  * XPCMSOUT1
  * XPWMECLK
  * XPWMTOUT0
  * XPWMTOUT1
  * XI2CSCL
  * XI2CSDA
  * XURXD1
  * XUTXD1
  * XUCTSN1
  * XURTSN1

## List B ##
(signals of which the name is known but it is not known where on UPC701 they connect, please provide pin name on UPC701)
  * PWR\_SCL\_3.0V
  * PWR\_SDA\_3.0V
  * FM\_SCL\_3.0V
  * FM\_SDA\_3.0V
  * AP\_SCL\_3.0V
  * AP\_SDA\_3.0V
  * BT\_UART\_RXD
  * BT\_UART\_TXD
  * BT\_UART\_CTS
  * BT\_UART\_RTS
  * WLAN\_SDIO\_CMD
  * WLAN\_SDIO\_CLK
  * MSENSE\_IRQ
  * MSENSE\_RST
  * ACC\_INT
  * CAM\_FLASH\_SET
  * CAM\_FLASH\_EN

## List C ##
(Signals of which the name is know as well as the connection to UPC701. Please provide connection information to other components than UPC701)
  * USB\_SEL
  * TA\_SEL
  * AP\_SCL\_1.8V
  * AP\_SDL\_1.8V
  * CAM\_EN
  * EARPATH\_SEL
  * EAR\_CP\_CODEC\_SW
  * MAIN\_CP\_CODEC\_SW
  * 5M\_EN
  * VIBTONE\_EN
  * TV\_EN
  * DET\_3.5
  * PS\_VOUT\_30

## List D ##
(Signals of which the name is know but it is not known where they connect. Please provide all connection information of these signals)
  * RSTIN\_IN
  * AP\_PMIC\_EN
  * PM\_INT\_N
  * AP\_N\_RST\_IN
  * PWRON
  * AP\_PS\_HOLD
  * PS\_HOLD\_F
  * PHONE\_ON
  * MAX\_8906\_AMP\_EN
  * IF\_CON\_SENSE
  * AUDIO\_L
  * AUDIO\_R
  * MSM\_VOICE\_P
  * MSM\_VOICE\_N
  * EAROUT\_L
  * EAROUT\_R
  * SPK\_OUT\_N
  * SPK\_OUT\_P