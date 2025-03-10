---
UID: NS:windns.DNS_NSEC_DATAW
title: DNS_NSEC_DATAW (windns.h)
description: Represents an NSEC resource record (RR) as specified in section 4 of RFC 4034. (Unicode)
helpviewer_keywords: ["*PDNS_NSEC_DATA","*PDNS_NSEC_DATAW","DNS_NSEC_DATA","DNS_NSEC_DATA structure [DNS]","DNS_NSEC_DATAW","PDNS_NSEC_DATA","PDNS_NSEC_DATA structure pointer [DNS]","dns.dns_nsec_data","windns/DNS_NSEC_DATA","windns/PDNS_NSEC_DATA"]
old-location: dns\dns_nsec_data.htm
tech.root: DNS
ms.assetid: ea446732-bc6a-4597-b164-11bfd77c07f2
ms.date: 12/05/2018
ms.keywords: '*PDNS_NSEC_DATA, *PDNS_NSEC_DATAW, DNS_NSEC_DATA, DNS_NSEC_DATA structure [DNS], DNS_NSEC_DATAW, PDNS_NSEC_DATA, PDNS_NSEC_DATA structure pointer [DNS], dns.dns_nsec_data, windns/DNS_NSEC_DATA, windns/PDNS_NSEC_DATA'
req.header: windns.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: Windows Server 2008 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: DNS_NSEC_DATAW, *PDNS_NSEC_DATAW
req.redist: 
ms.custom: 19H1
f1_keywords:
 - PDNS_NSEC_DATAW
 - windns/PDNS_NSEC_DATAW
 - DNS_NSEC_DATAW
 - windns/DNS_NSEC_DATAW
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Windns.h
api_name:
 - DNS_NSEC_DATA
---

# DNS_NSEC_DATAW structure


## -description

The <b>DNS_NSEC_DATA</b> structure represents an NSEC resource record (RR) as specified in section 4 of <a href="https://www.ietf.org/rfc/rfc4034.txt">RFC 4034</a>.

## -struct-fields

### -field pNextDomainName

A pointer to a string that represents the authoritative owner name of the next domain in the canonical ordering of the zone as specified in section 4.1.1 of <a href="https://www.ietf.org/rfc/rfc4034.txt">RFC 4034</a>.

### -field wTypeBitMapsLength

The length, in bytes, of <b>TypeBitMaps</b>.

### -field wPad

Reserved. Do not use.

### -field size_is

### -field size_is.wTypeBitMapsLength

### -field TypeBitMaps

A <b>BYTE</b> array that contains a bitmap that specifies which RR types are supported by the NSEC RR owner. Each bit in the array corresponds to a <a href="/windows/desktop/DNS/dns-constants">DNS Record Type</a> as defined in section in section 4.1.2 of <a href="https://www.ietf.org/rfc/rfc4034.txt">RFC 4034</a>.

## -remarks

The 
<b>DNS_NSEC_DATA</b> structure is used in conjunction with the 
<a href="/windows/win32/api/windns/ns-windns-dns_recorda">DNS_RECORD</a> structure to programmatically manage DNS entries.





> [!NOTE]
> The windns.h header defines DNS_NSEC_DATA as an alias that automatically selects the ANSI or Unicode version of this function based on the definition of the UNICODE preprocessor constant. Mixing usage of the encoding-neutral alias with code that is not encoding-neutral can lead to mismatches that result in compilation or runtime errors. For more information, see [Conventions for Function Prototypes](/windows/win32/intl/conventions-for-function-prototypes).

## -see-also

<a href="/windows/desktop/DNS/dns-structures">DNS Structures</a>



<a href="/windows/win32/api/windns/ns-windns-dns_recorda">DNS_RECORD</a>

