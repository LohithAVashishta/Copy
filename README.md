+----------------+
 SyslogStatus   
+----------------+
 - sectionG: SectionG 
+----------------+
 + SyslogStatus(name: Names, status: Status, issues: String) 
 + getSectionG(): SectionG 
 + setSectionG(sectionG: SectionG): void 
 + SyslogStatus() 
 + toString(): String 
+----------------+

+----------------+
 TwstftOffset   
+----------------+
 - sectionC: SectionC 
 - issues: String 
+----------------+
 + TwstftOffset(name: Names, value: Double, issues: String) 
 + addSectionC(sectionC: SectionC): void 
 + toString(): String 
 + getSectionC(): SectionC 
 + getIssues(): String 
 + TwstftOffset() 
 + setSectionC(sectionC: SectionC): void 
 + setIssues(issues: String): void 
+----------------+

+------------+
 Uere       
+------------+
 - satellite: String 
 - chain: String 
+------------+
 + Uere(server: String, location: String, value: Double, chain: String, satellite: String) 
 + getSatellite(): String 
 + getChain(): String 
 + setSatellite(satellite: String): void 
 + setChain(chain: String): void 
 + toString(): String 
 + Uere() 
+------------+

+----------------+
 UserPosition   
+----------------+
 (No additional attributes) 
+----------------+
 + UserPosition(server: String, location: String, value: Double) 
 + toString(): String 
 + UserPosition() 
+----------------+
