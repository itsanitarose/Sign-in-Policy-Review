
# Sign-in Policy Review

## 🎫 The Ticket
It's 16 November 2026, my seventh week on the security team at Northwind Health. The company's sign-in rules were set up quickly and have never been revisited. This week's request is to review a day of sign-in activity and propose better rules without locking people out.

My manager writes:

> Our sign-in rules were set up quickly and never revisited. Here's what we have today and a day of sign-in activity. I need to know which events worry you, and a better set of rules I can take to the IT director. Remember the front-desk staff at our clinics can't use their own phones.

<BR>

Supporting Information: [sign-in log & current rules](Documents/01.%20Sign-in%20Log%20%26%20Current%20Rules.md)

<BR>


<table>
<tr>
<td>

**🛡️ Decision**



</td>
</tr>
</table>



<BR>

## What's the Risk?

Sign-in rules set up quickly and never reviewed often leave loopholes, weak default settings, or outdated login methods, and all are easy targets that can be exploited. Ours were set up that way. Yesterday's sign-in log shows where those gaps are already in use.

<BR>



## The Investigation

I checked yesterday's **15 sign-ins** against the **6 rules** we have now, both in [sign-in log & current rules](Documents/01.%20Sign-in%20Log%20%26%20Current%20Rules.md), then worked through four questions:

1. Which sign-in events need attention first?
2. How should the sign-in policies be improved?
3. How can front-desk staff sign in safely without personal phones?
4. How can the new policies be introduced without disrupting access?

<br>

## What I Found

Five sign-ins to open, in this order.

| Severity | Account | Risk |
| --- | --- | --- |
| 🔴 Critical | breakglass-02 | Emergency admin, no MFA, no alert. |
| 🟠 High | s.park | Possible session theft. Austin, then Singapore nine minutes later. |
| 🟠 High | j.chen | Finance mailbox over IMAP. MFA was impossible. |
| 🟡 Medium | t.nguyen-admin | SMS on a personal laptop. The account is an admin. |
| 🟡 Medium | v.santos | Partner VPN treated as identity. No MFA. |

**Not incidents.** k.malik at HQ, trusted location, managed device. Clinic tablet, MFA timed out because staff cannot use personal phones.

[02. Event Triage](Documents/02.%20Event%20Triage.md)

## Decisions & Recommendations

## Reflection & Next Steps

## Explore the Investigation
