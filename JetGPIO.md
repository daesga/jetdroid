# Introduction #

This is what we know about the Jet application porcessor GPIOs.

# GPIO map #
|	GPIO pin	|	Signal name	|	Jet GPIO	|	Confidence level	|
|:---------|:------------|:---------|:-----------------|
|	GPA(0)	  |	XURXD0	     |		        |		                |
|	GPA(1)	  |	XUTXD0	     |		        |		                |
|	GPA(2)	  |	XUCTSN0	    |	GPIO\_AP\_SCL	|		                |
|	GPA(3)	  |	XURTSN0	    |	GPIO\_AP\_SDA	|		                |
|	GPA(4)	  |	XURXD1	     |	GPIO\_BT\_UART\_RXD	|	?	               |
|	GPA(5)	  |	XUTXD1	     |	GPIO\_BT\_UART\_TXD	|	?	               |
|	GPA(6)	  |	XUCTSN1	    |	GPIO\_BT\_UART\_CTS	|	?	               |
|	GPA(7)	  |	XURTSN1	    |	GPIO\_BT\_UART\_RTS	|	?	               |
|		        |		           |		        |		                |
|	GPB(0)	  |	XURXD2	     |	GPIO\_PDA\_RXD // AP\_RXD	|		                |
|	GPB(1)	  |	XUTXD2	     |	GPIO\_PDA\_TXD // AP\_TXD	|		                |
|	GPB(2)	  |	XURXD3	     |	CAM\_I2C\_SCL	|		                |
|	GPB(3)	  |	XUTXD3	     |	CAM\_I2C\_SDA	|		                |
|	GPB(4)	  |	XIRSDBW	    |		        |		                |
|	GPB(5)	  |	XI2CSCL	    |	GPIO\_I2C0\_SCL	|		                |
|	GPB(6)	  |	XI2CSDA	    |	GPIO\_I2C0\_SDA	|		                |
|	GPB(7)	  |		           |		        |		                |
|		        |		           |		        |		                |
|	GPC(0)	  |	XSPIMISO0	  |	GPIO\_WLAN\_SDIO\_CMD	|	?	               |
|	GPC(1)	  |	XSPICLK0	   |	GPIO\_WLAN\_SDIO\_CLK	|	?	               |
|	GPC(2)	  |	XSPIMOSI0	  |		        |		                |
|	GPC(3)	  |	XSPICS0	    |		        |		                |
|	GPC(4)	  |	XSPIMISO1/XmmcCMD2	|	GPIO\_SDIO\_CMD	|	?	               |
|	GPC(5)	  |	XSPICLK1/XmmcCLK2	|	GPIO\_SDIO\_CLK	|	?	               |
|	GPC(6)	  |	XSPIMOSI1	  |		        |		                |
|	GPC(7)	  |	XSPICS1	    |		        |		                |
|		        |		           |		        |		                |
|	GPD(0)	  |	XPCMDCLK0	  |	GPIO\_I2S\_CLK	|		                |
|	GPD(1)	  |	XPCMEXTCLK0	|		        |		                |
|	GPD(2)	  |	XPCMFSYNC0	 |	GPIO\_I2S\_LRCLK AP\_I2S\_SYNC	|		                |
|	GPD(3)	  |	XPCMSIN0	   |	GPIO\_I2S\_DI	|		                |
|	GPD(4)	  |	XPCMSOUT0	  |	GPIO\_I2S\_DO	|		                |
|		        |		           |		        |		                |
|	GPE(0)	  |	XPCMDCLK1	  |		        |		                |
|	GPE(1)	  |	XPCMEXTCLK1	|		        |		                |
|	GPE(2)	  |	XPCMFSYNC1	 |		        |		                |
|	GPE(3)	  |	XPCMSIN1	   |	GPIO\_PWR\_I2C\_SCL	|		                |
|	GPE(4)	  |	XPCMSOUT1	  |	GPIO\_PWR\_I2C\_SDA	|		                |
|		        |		           |		        |		                |
|	GPF(0)	  |	XCICLK	     |	GPIO\_CAM\_MCLK	|	+	               |
|	GPF(1)	  |	XCIHREF	    |	GPIO\_CAM\_HSYNC	|	+	               |
|	GPF(2)	  |	XCIPCLK	    |	GPIO\_CAM\_PCLK	|	+	               |
|	GPF(3)	  |	XCIRSTN	    |	GPIO\_MCAM\_RST\_N	|	+	               |
|	GPF(4)	  |	XCIVSYNC	   |	GPIO\_CAM\_VSYNC	|	+	               |
|	GPF(5)	  |	XCIYDATA0	  |	GPIO\_CAM\_D\_0	|	+	               |
|	GPF(6)	  |	XCIYDATA1	  |	GPIO\_CAM\_D\_1	|	+	               |
|	GPF(7)	  |	XCIYDATA2	  |	GPIO\_CAM\_D\_2	|	+	               |
|	GPF(8)	  |	XCIYDATA3	  |	GPIO\_CAM\_D\_3	|	+	               |
|	GPF(9)	  |	XCIYDATA4	  |	GPIO\_CAM\_D\_4	|	+	               |
|	GPF(10)	 |	XCIYDATA5	  |	GPIO\_CAM\_D\_5	|	+	               |
|	GPF(11)	 |	XCIYDATA6	  |	GPIO\_CAM\_D\_6	|	+	               |
|	GPF(12)	 |	XCIYDATA7	  |	GPIO\_CAM\_D\_7	|	+	               |
|	GPF(13)	 |	XPWMECLK	   |		        |		                |
|	GPF(14)	 |	XPWMTOUT0	  |		        |		                |
|	GPF(15)	 |	XPWMTOUT1	  |	VIBTONE\_PWM	|	?	               |
|		        |		           |		        |		                |
|	GPG(0)	  |	XMMCCLK0	   |	GPIO\_TF\_CLK	|	++	              |
|	GPG(1)	  |	XMMCCMD0	   |	GPIO\_TF\_CMD	|	++	              |
|	GPG(2)	  |	XMMCDATA0\_0	|	GPIO\_TF\_D\_0	|	++	              |
|	GPG(3)	  |	XMMCDATA0\_1	|	GPIO\_TF\_D\_1	|	++	              |
|	GPG(4)	  |	XMMCDATA0\_2	|	GPIO\_TF\_D\_2	|	++	              |
|	GPG(5)	  |	XMMCDATA0\_3	|	GPIO\_TF\_D\_3	|	++	              |
|	GPG(6)	  |	XMMCCDN0	   |	GPIO\_TFLASH\_EN	|	++	              |
|		        |		           |		        |		                |
|	GPH(0)	  |	XMMCCLK1	   |	GPIO\_NAND\_CLK	|	?	               |
|	GPH(1)	  |	XMMCCMD1	   |	GPIO\_NAND\_CMD	|	?	               |
|	GPH(2)	  |	XMMCDATA1\_0	|	GPIO\_NAND\_D\_0	|	?	               |
|	GPH(3)	  |	XMMCDATA1\_1	|	GPIO\_NAND\_D\_1	|	?	               |
|	GPH(4)	  |	XMMCDATA1\_2	|	GPIO\_NAND\_D\_2	|	?	               |
|	GPH(5)	  |	XMMCDATA1\_3	|	GPIO\_NAND\_D\_3	|	?	               |
|	GPH(6)	  |	XMMCDATA1\_4/XmmcDAT2\_0	|	GPIO\_WLAN\_SDIO\_D\_0	|	?	               |
|	GPH(7)	  |	XMMCDATA1\_5/XmmcDAT2\_1	|	GPIO\_WLAN\_SDIO\_D\_1	|	?	               |
|	GPH(8)	  |	XMMCDATA1\_6/XmmcDAT2\_2	|	GPIO\_WLAN\_SDIO\_D\_2	|	?	               |
|	GPH(9)	  |	XMMCDATA1\_7/XmmcDAT2\_3	|	GPIO\_WLAN\_SDIO\_D\_3	|	?	               |
|		        |		           |		        |		                |
|	GPI(0)	  |	XVVD0	      |	GPIO\_LCD\_B\_0	|	++	              |
|	GPI(1)	  |	XVVD1	      |	GPIO\_LCD\_B\_1	|	++	              |
|	GPI(2)	  |	XVVD2	      |	GPIO\_LCD\_B\_2	|	++	              |
|	GPI(3)	  |	XVVD3	      |	GPIO\_LCD\_B\_3	|	++	              |
|	GPI(4)	  |	XVVD4	      |	GPIO\_LCD\_B\_4	|	++	              |
|	GPI(5)	  |	XVVD5	      |	GPIO\_LCD\_B\_5	|	++	              |
|	GPI(6)	  |	XVVD6	      |	GPIO\_LCD\_B\_6	|	++	              |
|	GPI(7)	  |	XVVD7	      |	GPIO\_LCD\_B\_7	|	++	              |
|	GPI(8)	  |	XVVD8	      |	GPIO\_LCD\_G\_0	|	++	              |
|	GPI(9)	  |	XVVD9	      |	GPIO\_LCD\_G\_1	|	++	              |
|	GPI(10)	 |	XVVD10	     |	GPIO\_LCD\_G\_2	|	++	              |
|	GPI(11)	 |	XVVD11	     |	GPIO\_LCD\_G\_3	|	++	              |
|	GPI(12)	 |	XVVD12	     |	GPIO\_LCD\_G\_4	|	++	              |
|	GPI(13)	 |	XVVD13	     |	GPIO\_LCD\_G\_5	|	++	              |
|	GPI(14)	 |	XVVD14	     |	GPIO\_LCD\_G\_6	|	++	              |
|	GPI(15)	 |	XVVD15	     |	GPIO\_LCD\_G\_7	|	++	              |
|		        |		           |		        |		                |
|	GPJ(0)	  |	XVVD16	     |	GPIO\_LCD\_R\_0	|	++	              |
|	GPJ(1)	  |	XVVD17	     |	GPIO\_LCD\_R\_1	|	++	              |
|	GPJ(2)	  |	XVVD18	     |	GPIO\_LCD\_R\_2	|	++	              |
|	GPJ(3)	  |	XVVD19	     |	GPIO\_LCD\_R\_3	|	++	              |
|	GPJ(4)	  |	XVVD20	     |	GPIO\_LCD\_R\_4	|	++	              |
|	GPJ(5)	  |	XVVD21	     |	GPIO\_LCD\_R\_5	|	++	              |
|	GPJ(6)	  |	XVVD22	     |	GPIO\_LCD\_R\_6	|	++	              |
|	GPJ(7)	  |	XVVD23	     |	GPIO\_LCD\_R\_7	|	++	              |
|	GPJ(8)	  |	XVHSYNC	    |	GPIO\_LCD\_HSYNC	|	++	              |
|	GPJ(9)	  |	XVVSYNC	    |	GPIO\_LCD\_VSYNC	|	++	              |
|	GPJ(10)	 |	XVDEN	      |	GPIO\_LCD\_DE	|	++	              |
|	GPJ(11)	 |	XVVCLK	     |	GPIO\_LCD\_CLK	|	++	              |
|		        |		           |		        |		                |
|	GPK(0)	  |	XHIDATA0	   |	GPIO\_TA\_SEL	|	++	              |
|	GPK(1)	  |	XHIDATA1	   |	GPIO\_CAM\_EN	|	++	              |
|	GPK(2)	  |	XHIDATA2	   |	GPIO\_EARPATH\_SEL	|	++	              |
|	GPK(3)	  |	XHIDATA3	   |	GPIO\_EAR\_CP\_CODEC\_SW	|	++	              |
|	GPK(4)	  |	XHIDATA4	   |	GPIO\_MAIN\_CP\_CODEC\_SW	|	++	              |
|	GPK(5)	  |	XHIDATA5	   |	GPIO\_FM\_RST	|	++	              |
|	GPK(6)	  |	XHIDATA6	   |		        |		                |
|	GPK(7)	  |	XHIDATA7	   |	GPIO\_PHONE\_RST\_N	|		                |
|	GPK(8)	  |	XHIDATA8	   |	GPIO\_KEYSENSE\_0	|	++	              |
|	GPK(9)	  |	XHIDATA9	   |	GPIO\_KEYSENSE\_1	|	++	              |
|	GPK(10)	 |	XHIDATA10	  |	GPIO\_KEYSENSE\_2	|	++	              |
|	GPK(11)	 |	XHIDATA11	  |	GPIO\_KEYSENSE\_3	|	++	              |
|	GPK(12)	 |	XHIDATA12	  |		        |		                |
|	GPK(13)	 |	XHIDATA13	  |		        |		                |
|	GPK(14)	 |	XHIDATA14	  |		        |		                |
|	GPK(15)	 |	XHIDATA15	  |	GPIO\_VMSMP\_26V	|		                |
|		        |		           |		        |		                |
|	GPL(0)	  |	XHIADDR0	   |	GPIO\_KEYSCAN\_0	|	++	              |
|	GPL(1)	  |	XHIADDR1	   |	GPIO\_KEYSCAN\_1	|	++	              |
|	GPL(2)	  |	XHIADDR2	   |	GPIO\_KEYSCAN\_2	|	++	              |
|	GPL(3)	  |	XHIADDR3	   |	GPIO\_5M\_EN	|	++	              |
|	GPL(4)	  |	XHIADDR4	   |	GPIO\_VIBTONE\_EN	|	++	              |
|	GPL(5)	  |	XHIADDR5	   |	GPIO\_USB\_SEL	|	++	              |
|	GPL(6)	  |	XHIADDR6	   |	GPIO\_TV\_EN	|	++	              |
|	GPL(7)	  |	XHIADDR7	   |	GPIO\_TOUCH\_EN	|	++	              |
|	GPL(8)	  |	XHIADDR8	   |	GPIO\_T\_FLASH\_DETECT	|	++	              |
|	GPL(9)	  |	XHIADDR9	   |	GPIO\_DET\_35	|	++	              |
|	GPL(10)	 |	XHIADDR10	  |	GPIO\_FM\_INT	|	++	              |
|	GPL(11)	 |	XHIADDR11	  |	GPIO\_EXTWKUP	|	++	              |
|	GPL(12)	 |	XHIADDR12	  |	GPIO\_PS\_VOUT\_30	|	++	              |
|	GPL(13)	 |	XHIDATA16	  |		        |		                |
|	GPL(14)	 |	XHIDATA17	  |		        |		                |
|		        |		           |		        |		                |
|	GPM(0)	  |	XHICSN	     |	GPIO\_FM\_I2C\_SCL	|	+	               |
|	GPM(1)	  |	XHICSN\_MAIN	|	GPIO\_FM\_I2C\_SDA	|	+	               |
|	GPM(2)	  |	XHICSN\_SUB	|	GPIO\_WLAN\_HOST\_WAKE	|	++	              |
|	GPM(3)	  |	XHIWEN	     |	GPIO\_BT\_HOST\_WAKE	|	++	              |
|	GPM(4)	  |	XHIOEN	     |	GPIO\_OJ\_MOTION	|		                |
|	GPM(5)	  |	XHIINTR	    |	GPIO\_MSENSE\_RST\_N	|		                |
|		        |		           |		        |		                |
|	GPN(0)	  |	XEINT0	     |	GPIO\_ONEDRAM\_INT\_N	|		                |
|	GPN(1)	  |	XEINT1	     |		        |		                |
|	GPN(2)	  |	XEINT2	     |	GPIO\_MSENSE\_INT	|		                |
|	GPN(3)	  |	XEINT3	     |	GPIO\_ACC\_INT	|		                |
|	GPN(4)	  |	XEINT4	     |	GPIO\_HALL\_SW	|		                |
|	GPN(5)	  |	XEINT5	     |	GPIO\_POWER\_N	|		                |
|	GPN(6)	  |	XEINT6	     |		        |		                |
|	GPN(7)	  |	XEINT7	     |	GPIO\_PHONE\_ACTIVE	|		                |
|	GPN(8)	  |	XEINT8	     |		        |		                |
|	GPN(9)	  |	XEINT9	     |	GPIO\_JACK\_INT\_N	|		                |
|	GPN(10)	 |	XEINT10	    |		        |		                |
|	GPN(11)	 |	XEINT11	    |	GPIO\_EAR\_SEND\_END	|		                |
|	GPN(12)	 |	XEINT12	    |	GPIO\_RESOUT\_N	|		                |
|	GPN(13)	 |	XEINT13	    |	GPIO\_BOOT\_EINT13	|		                |
|	GPN(14)	 |	XEINT14	    |	GPIO\_BOOT\_EINT14	|		                |
|	GPN(15)	 |	XEINT15	    |	GPIO\_BOOT\_EINT15	|		                |
|		        |		           |		        |		                |
|	GPO(0)	  |	Xm0ADDR0	   |	N.C.	    |	++	              |
|	GPO(1)	  |	Xm0ADDR1	   |	N.C.	    |	++	              |
|	GPO(2)	  |	Xm0ADDR2	   |	N.C.	    |	++	              |
|	GPO(3)	  |	Xm0ADDR3	   |	N.C.	    |	++	              |
|	GPO(4)	  |	Xm0ADDR4	   |	N.C.	    |	++	              |
|	GPO(5)	  |	Xm0ADDR5	   |	N.C.	    |	++	              |
|	GPO(6)	  |	Xm0ADDR6	   |	GPIO\_LCD\_CS\_N	|	++	              |
|	GPO(7)	  |	Xm0ADDR7	   |	GPIO\_LCD\_SDI	|	++	              |
|	GPO(8)	  |	Xm0ADDR8	   |	GPIO\_AP\_SCL\_1\_8V	|	++	              |
|	GPO(9)	  |	Xm0ADDR9	   |	GPIO\_AP\_SDA\_1\_8V	|	++	              |
|	GPO(10)	 |	Xm0ADDR10	  |	GPIO\_LCD\_RST\_N	|	++	              |
|	GPO(11)	 |	Xm0ADDR11	  |	GPIO\_LCD\_DET	|	++	              |
|	GPO(12)	 |	Xm0ADDR12	  |	GPIO\_LCD\_SCLK	|	++	              |
|	GPO(13)	 |	Xm0ADDR13	  |	N.C.	    |	++	              |
|	GPO(14)	 |	Xm0ADDR14	  |	GPIO\_REV\_1	|	++	              |
|	GPO(15)	 |	Xm0ADDR15	  |	GPIO\_REV\_2	|	++	              |
|		        |		           |		        |		                |
|	GPP(13)	 |	Xm0OEata	   |	GPIO\_PDA\_PS\_HOLD	|		                |
|		        |		           |		        |		                |
|	GPQ(7)	  |	Xm0ADDR17	  |	N.C.	    |	++	              |
|	GPQ(8)	  |	Xm0ADDR16	  |	GPIO\_REV\_3	|	++	              |
|		        |		           |		        |		                |
|	Xm0DATA0	|		           |	N.C.	    |	++	              |
|	Xm0DATA1	|		           |	N.C.	    |	++	              |
|	Xm0DATA2	|		           |	N.C.	    |	++	              |
|	Xm0DATA3	|		           |	N.C.	    |	++	              |
|	Xm0DATA4	|		           |	N.C.	    |	++	              |

Confidence levels:
++ verified, + very likely, ? needs to be verified