Mobile Network Evolution: From GSM to LTE - Architecture, Performance, and Technology Transitions
Author: Ajibawo, Oladipo Oluyemisi

Date: November 2015



Overview
This research article provides a comprehensive comparative review of mobile wireless network evolution from second-generation GSM through third-generation UMTS and HSPA to fourth-generation LTE. The study covers network architecture, modulation methods, data rates, traffic classes, and the key interface and component changes across each technology generation.

Table of Contents
·	Section 1: Introduction
·	Section 2: GSM vs. UMTS
·	Section 3: High Speed Packet Access (HSPA)
·	Section 4: Long Term Evolution (LTE)
·	Generation Comparison
·	Key Findings
·	References

Section 1: Introduction
Mobile communication has evolved through five generations, each delivering substantial improvements in data rates, spectral efficiency, and architectural simplicity.
Generation	Technology	Era	Key Characteristic
1G	Analogue cellular	1980s	Voice only, no data
2G	GSM, CDMA	1990s	Digital voice, SMS, low-speed data
3G	UMTS, CDMA2000	2000s	Mobile broadband, video calling
3.5G	HSPA, HSPA+	2005-2010	Enhanced data rates, low latency
4G	LTE, LTE-Advanced	2010s	All-IP, broadband, MIMO

3G ITU-IMT-2000 requirements specified: 144 kbps at mobile speeds, 384 kbps at pedestrian speeds, and 2 Mbps indoors.

Section 2: GSM vs. UMTS
Modulation and Access Methods
Feature	GSM	UMTS
Multiple access	TDMA	WCDMA
Modulation	GMSK	QPSK (uplink), 16QAM (HSDPA)
Frequency	850/900/1800/1900 MHz	1900-2025 MHz, 2110-2200 MHz
Max data rate	14.4 kbps (circuit)	2 Mbps (indoor) / 384 kbps (outdoor)
Channel width	200 kHz (8 time slots)	5 MHz (WCDMA)

Traffic Classes
GSM:
1.	Signalling (16k, 32k, 64k)
2.	Voice and Fax
3.	Data: GPRS, EDGE, Extended Data
UMTS:
1.	Conversational (voice, video telephony, video gaming)
2.	Streaming (multimedia, VOD, webcast)
3.	Interactive (web browsing, gaming, database access)
4.	Background (email, SMS, file downloading)
Network Architecture Comparison
GSM Architecture:
·	Mobile Station (MS): SIM + ME, IMEI and IMSI identifiers
·	Base Station Subsystem (BSS): BTS (radio transmitters) + BSC (call maintenance)
·	Network Subsystem: MSC, HLR, VLR, AuC, EIR
UMTS Architecture (Key Components):
·	UE (User Equipment)
·	UTRAN: WCDMA radio access network with RNC and Node-B BSs
·	Core Network (CN): PS domain (SGSN, GGSN) and CS domain (MSC/VLR, GMSC)
3GPP Release 4 Change: MSC/VLR and GMSC split into (G)MSC Server and Media Gateway (MGW), separating call control from media switching.

Section 3: HSPA
High Speed Packet Access combines HSDPA (Release 5) and HSUPA (Release 6) to deliver substantially higher data rates over existing WCDMA networks.
Data Rate Comparison
System	GSM	GPRS	EDGE	3G (R99)	HSDPA
Typical Max. (Kbit/s)	9.6	50	130	384	2,048+
Theoretical Max. (Kbit/s)	14.4	170	384	2,048	14,400

HSDPA (3GPP Release 5)
Key improvements over UMTS:
·	16QAM higher-order modulation for improved spectral efficiency
·	Adaptive Modulation and Coding (AMC): modulation adapts dynamically to channel conditions
·	Hybrid ARQ (HARQ): fast retransmission at the physical layer
·	Maximum theoretical downlink rate: 14.4 Mbit/s
Advantages:
·	Shorter frame lengths for faster response to channel degradation
·	Well suited to variable and bursty bandwidth demands
·	Dedicated high-speed downlink shared channel
HSUPA (3GPP Release 6)
Key improvements:
·	Maximum uplink rate: 5.8 Mbps (Enhanced Uplink Dedicated Channel, E-DCH)
·	Supports Soft Handover and Hybrid ARQ
·	Fast packet scheduling with multicode transmission
·	Improves symmetric services: email, video gaming, live streaming
3GPP Releases 7 and 8 (HSPA+)
·	Release 7 (HSPA+): Flatter architecture, enhanced VoIP capacity, discontinuous transmission (mobile transmitter shuts down when idle)
·	Release 8 (LTE): Reduces network elements from four (Release 6) to two; further increases data rates and reduces latency
·	LTE performance target: 2 to 4 times the performance of HSPA Release 6

Section 4: LTE
LTE (Long Term Evolution), the 3GPP Release 8 specification, provides a fully packet-switched network with high data rates, low latency, and flexible spectrum usage.
LTE Architecture Components
         PDN-GW ─── Internet
            │ S5
         Serving-GW
            │ S11              S6
           MME ──────────────── HSS
            │ S1
         eNode-B ─── X2 ─── eNode-B
            │
        Mobile Device (UE)

Component Functions
Component	Function
eNode-B	Air interface, resource scheduling, QoS enforcement, mobility management, interference coordination
S1 interface	eNode-B to core network: operational signalling and user signalling
X2 interface	eNode-B to eNode-B: handover coordination and interference management
MME	Authentication, bearer establishment, handover support, GSM/UMTS interworking
Serving Gateway (S-GW)	User data tunnel management between eNode-Bs and PDN-GW
PDN Gateway (PDN-GW)	Internet gateway, IP address assignment, enterprise intranet access
HSS	Home Subscriber Server: centralised user database for authentication and subscriber data

LTE User Equipment (UE) Categories
Category	Downlink MIMO	Peak Downlink	Notes
1-4	2x2 MIMO	Up to 150 Mbps	All support 64-QAM downlink
5	4x4 MIMO (future)	Up to 300 Mbps	Advanced transmission

All LTE UEs support 64-QAM in the downlink and 16-QAM in the uplink as minimum requirements.
LTE vs. HSPA
Feature	HSPA R6	LTE (R8)
Network elements	4	2
Architecture	Hierarchical (RNC)	Flat (eNode-B direct)
Latency	~50 ms	<10 ms
Peak downlink	14.4 Mbps	150+ Mbps
Spectrum flexibility	5 MHz fixed	1.4 to 20 MHz
Handover control	RNC	eNode-B + MME


Key Findings
·	The elimination of the RNC in LTE creates a flatter architecture that reduces latency and simplifies handover procedures
·	3GPP Release 4's separation of the MSC into server and MGW components established the softswitch model that LTE's MME builds upon
·	HSDPA's introduction of AMC and HARQ at the physical layer fundamentally changed how link adaptation is handled in mobile networks
·	LTE's eNode-B assumes functions previously distributed across the RNC and Node-B, centralising radio resource management
·	The PDN-GW IP address assignment function enables seamless session continuity during handovers and roaming

References
·	3GPP Standard (2008). Ultra-Long Term Evolution (LTE) and 3GPP System Architecture Evolution (SAE). March.
·	Abdullah, O., Enan, M., Babiker, A. and Mustafa, N. (2014). Comparative Study between UMTS, HSDPA and HSUPA. Journal of Electronics and Communication Engineering, 9(4), pp. 21-30.
·	Atayero, A., Luka, K., Orya, K. and Iruem, J. (2011). 3GPP Long Term Evolution: Architecture, Protocols, and Interface. International Journal of Information and Communication Technology Research (IJICT), November, 1(7).
·	Chakraborty, A. (2013). A Study on Third Generation Mobile Technology (3G). International Journal of Innovative Technology and Adaptive Management (IJITAM), November, 1(2).
·	Dahlman, E., Parkvall, S. and Skold, J. (2011). 4G LTE/LTE-Advanced for Mobile Broadband. 1st edn. United Kingdom: Elsevier.
·	Eberspacher, J., Vogel, H., Bettstetter, C. and Hartmann, C. (2009). GSM Architecture, Protocols and Services. 3rd edn. Chichester: John Wiley and Sons, Ltd.
·	Holma, H. and Toskala, A. (2000). WCDMA for UMTS. Chichester: John Wiley and Sons, Ltd.
·	Holma, H. and Toskala, A. (2006). HSDPA/HSUPA for UMTS: High Speed Radio Access for Mobile Communications. West Sussex: John Wiley and Sons, Ltd.
·	Kumar, A., Liu, Y. and Sengupta, J. (2010). Evolution of Mobile Wireless Networks: 1G to 4G. IJECT, December, 1(1).
·	Sauter, M. (2011). From GSM to LTE: An Introduction of Mobile Networks and Mobile Broadband. 2nd edn. West Sussex: John Wiley and Sons, Ltd.
·	Sesia, S., Toufik, I. and Baker, M. (2011). LTE: The UMTS Long Term Evolution From Theory to Practice. 2nd edn. West Sussex: John Wiley and Sons, Ltd.

Ajibawo, Oladipo Oluyemisi

