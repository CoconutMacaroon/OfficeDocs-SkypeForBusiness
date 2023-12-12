---
title: Require end-to-end encryption for sensitive Teams meetings
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
ms.topic: article
ms.service: msteams
ms.reviewer: maahma
ms.date: 12/11/2023
audience: admin
ms.localizationpriority: medium
f1.keywords:
- NOCSH
ms.collection: 
  - m365solution-compliantmeetings
  - m365initiative-meetings
  - highpri
  - Tier1
appliesto: 
  - Microsoft Teams
description: Learn how to enable end-to-end encryption for Teams meetings.
---

# Require end-to-end encryption for sensitive Teams meetings

[!INCLUDE[Teams Premium ECM](includes/teams-premium-ecm.md)]

End-to-end encryption is the encryption of information at its origin and decryption at its intended destination without the ability for intermediate nodes to decrypt. When meetings in Teams are end-to-end encrypted, nobody except for the participants in the meeting can hear or see the communication. No other party, including Microsoft, has access to the decrypted conversation.

End-to-end encrypted meetings can be made between two parties when: the parties are using the latest version of the Teams desktop client for Windows or Mac or they are on a mobile device with the latest update for iOS and Android.

Web, Virtual Desktop (VDI), Cloud Video Interoperability(CVI), and Android Teams Room devices aren't currently supported. Participants trying to join an end-to-end encrypted meeting from one of these platforms are blocked.

A maximum of 200 participants can attend an end-to-end encrypted meeting. If the first participant joins from a Surface Hub or Windows Teams Room device, the maximum number of participants is 50.

> [!Note]
> End-to-end meeting encryption requires Teams Premium.

If you don't enable end-to-end encryption, Teams still secures meetings using encryption based on industry standards. Data exchanged during meetings is always secure while in transit and at rest. For more information, see [Media encryption for Teams](teams-security-guide.md#media-encryption).

During an end-to-end encrypted meeting, Teams secures the following features:

- Audio

- Video

- Screen sharing

[Encryption in Microsoft 365](/microsoft-365/compliance/encryption) protects chat, file sharing, presence, and other content in the meeting. Apps, avatars, reactions, chat, and Q&A aren't end-to-end encrypted.

The following features aren't available during an end-to-end encrypted meeting:

- Recording

- Live captions and transcription

- Together mode, companion mode, large gallery

- Breakout rooms

- PowerPoint Live

- Excel Live

If your organization uses compliance recording for 1:1 calls, end-to-end encryption isn't available. An individual who needs compliance recording can't join an end-to-end encrypted meeting. For more info on how Teams supports compliance recording, see [Introduction to Teams policy-based recording for callings & meetings](teams-recording-policy.md).

## Enable end-to-end encryption for meetings

By default, end-to-end encryption for meetings isn't enabled. You can enable it by using a Teams admin enhanced encryption policy.

Once end-to-end encryption is enabled, meeting organizers have the option of choosing end-to-end encryption then they create a meeting, including channel meetings. You can also enforce end-to-end encryption by using a meeting template. Note that sensitivity labels can enforce end-to-end encryption even if the Teams admin enhanced encryption policy isn't enabled for the meeting organizer.

To enable end-to-end encryption for meetings

1. In the Teams admin center, select **Enhanced encryption policy**.

1. Select the policy you want to update.

1. Set **End-to-end meeting encryption**, to **Not enabled, but users can enable**.

1. Select **Save**.

## Related topics

[Configure Teams meetings with three tiers of protection](configure-meetings-three-tiers-protection.md)

[Use end-to-end encryption for one-to-one Microsoft Teams calls](teams-end-to-end-encryption.md)
