--------------------------------
|   NavicPerformanceDetails    |
--------------------------------
| - id: Long                   |
| - sectionA: SectionA         |
| - sectionB: SectionB         |
| - sectionC: SectionC         |
| - sectionD: SectionD         |
| - sectionE: SectionE         |
| - sectionF: SectionF         |
| - sectionG: SectionG         |
| - sectionH: SectionH         |
| - createdAt: LocalDateTime   |
| - modifiedAt: LocalDateTime  |
--------------------------------
| + NavicPerformanceDetails()  |
| + NavicPerformanceDetails(   |
|     sectionA: SectionA,      |
|     sectionB: SectionB,      |
|     sectionC: SectionC,      |
|     sectionD: SectionD,      |
|     sectionE: SectionE,      |
|     sectionF: SectionF,      |
|     sectionG: SectionG,      |
|     sectionH: SectionH,      |
|     createdAt: LocalDateTime,|
|     modifiedAt: LocalDateTime|
|   )                          |
| + addSectionA(sectionA: SectionA)|
| + addSectionB(sectionB: SectionB)|
| + addSectionC(sectionC: SectionC)|
| + addSectionD(sectionD: SectionD)|
| + addSectionE(sectionE: SectionE)|
| + addSectionF(sectionF: SectionF)|
| + addSectionG(sectionG: SectionG)|
| + addSectionH(sectionH: SectionH)|
| + getId(): Long               |
| + getSectionA(): SectionA     |
| + getSectionB(): SectionB     |
| + getSectionC(): SectionC     |
| + getSectionD(): SectionD     |
| + getSectionE(): SectionE     |
| + getSectionF(): SectionF     |
| + getSectionG(): SectionG     |
| + getSectionH(): SectionH     |
| + getCreatedAt(): LocalDateTime |
| + getModifiedAt(): LocalDateTime |
| + setId(id: Long)             |
| + setSectionA(sectionA: SectionA)|
| + setSectionB(sectionB: SectionB)|
| + setSectionC(sectionC: SectionC)|
| + setSectionD(sectionD: SectionD)|
| + setSectionE(sectionE: SectionE)|
| + setSectionF(sectionF: SectionF)|
| + setSectionG(sectionG: SectionG)|
| + setSectionH(sectionH: SectionH)|
| + setCreatedAt(createdAt: LocalDateTime) |
| + setModifiedAt(modifiedAt: LocalDateTime) |
| + toString(): String          |
--------------------------------








--------------------------------
|     NavigationArchival       |
--------------------------------
| - sectionB: SectionB         |
--------------------------------
| + NavigationArchival(        |
|     name: ArchivalName,      |
|     status: Status,          |
|     size: String             |
|   )                          |
| + addSectionB(sectionB: SectionB)|
| + getSectionB(): SectionB     |
| + setSectionB(sectionB: SectionB)|
| + toString(): String          |
--------------------------------








