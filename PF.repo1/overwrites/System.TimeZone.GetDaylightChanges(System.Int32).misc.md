---
uid: System.TimeZone.GetDaylightChanges(System.Int32)
additional_notes.usage: *content
---

<p>Because the <xref href="System.TimeZone"></xref> class supports only one daylight saving time adjustment rule, the <xref href="System.TimeZone.GetDaylightChanges(System.Int32)"></xref> method applies the current adjustment rule to any year, regardless of whether the adjustment rule actually applies to that year. Assuming that the operating system itself has accurate data for a particular year, a more accurate result is available by working with the array of <xref href="System.TimeZoneInfo.AdjustmentRule"></xref> objects returned by the <xref href="System.TimeZoneInfo.GetAdjustmentRules"></xref> method. The <xref href="System.Globalization.DaylightTime.Start"></xref>, <xref href="System.Globalization.DaylightTime.End"></xref>, and <xref href="System.Globalization.DaylightTime.Delta"></xref> properties correspond to the <xref href="System.TimeZoneInfo.AdjustmentRule.DateStart"></xref>, <xref href="System.TimeZoneInfo.AdjustmentRule.DateEnd"></xref>, and <xref href="System.TimeZoneInfo.AdjustmentRule.DaylightDelta"></xref> properties.</p>


