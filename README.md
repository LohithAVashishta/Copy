+-----------------+
 StandardFile    
+-----------------+
 - id: Long      
 - fileName: String   
 - standardFileStatus: StandardFileStatus   
 - status: Boolean    
+-----------------+
 + StandardFile(fileName: String, status: Boolean) 
 + addStandardFileStatus(standardFileStatus: StandardFileStatus): void 
 + getId(): Long 
 + getFileName(): String 
 + getStandardFileStatus(): StandardFileStatus 
 + getStatus(): Boolean 
 + setId(id: Long): void 
 + setFileName(fileName: String): void 
 + setStandardFileStatus(standardFileStatus: StandardFileStatus): void 
 + setStatus(status: Boolean): void 
 + StandardFile() 
 + StandardFile(id: Long, fileName: String, standardFileStatus: StandardFileStatus, status: Boolean) 
 + toString(): String 
+-----------------+

+-----------------------+
 StandardFileStatus    
+-----------------------+
 - id: Long            
 - sectionB: SectionB  
 - availableDocuments: List<StandardFile> 
+-----------------------+
 + StandardFileStatus(availableDocuments: List<StandardFile>) 
 + addStandardFile(standardFile: StandardFile): void 
 + getId(): Long 
 + getSectionB(): SectionB 
 + getAvailableDocuments(): List<StandardFile> 
 + setId(id: Long): void 
 + setSectionB(sectionB: SectionB): void 
 + setAvailableDocuments(availableDocuments: List<StandardFile>): void 
 + StandardFileStatus() 
 + toString(): String 
+-----------------------+

+------------+
 Station    
+------------+
 - id: Long 
 - enable: Boolean 
 - baseMaintenance: BaseMaintenance 
 - name: String 
+------------+
 + Station(name: String) 
 + getId(): Long 
 + getEnable(): Boolean 
 + getBaseMaintenance(): BaseMaintenance 
 + getName(): String 
 + setId(id: Long): void 
 + setEnable(enable: Boolean): void 
 + setBaseMaintenance(baseMaintenance: BaseMaintenance): void 
 + setName(name: String): void 
 + Station() 
 + Station(id: Long, enable: Boolean, baseMaintenance: BaseMaintenance, name: String) 
 + toString(): String 
+------------+

+-------------------+
 StnLookAngle      
+-------------------+
 - id: Long        
 - location: String 
 - availableTill: LocalDateTime 
 - enable: Boolean 
 - sectionH: SectionH 
+-------------------+
 + StnLookAngle(location: String, availableTill: LocalDateTime, enable: Boolean) 
 + addSectionH(sectionH: SectionH): void 
 + getId(): Long 
 + getLocation(): String 
 + getAvailableTill(): LocalDateTime 
 + getEnable(): Boolean 
 + getSectionH(): SectionH 
 + setId(id: Long): void 
 + setLocation(location: String): void 
 + setAvailableTill(availableTill: LocalDateTime): void 
 + setEnable(enable: Boolean): void 
 + setSectionH(sectionH: SectionH): void 
 + StnLookAngle() 
 + toString(): String 
+-------------------+

+-----------------+
 StorageIssues   
+-----------------+
 - sectionB: SectionB 
 - nsopStorageSet: List<NsopStorageStatus> 
+-----------------+
 + StorageIssues(nsopStorage: Set<NsopStorageStatus>, issues: String) 
 + addNsopStorageStatus(nsopStorageStatus: NsopStorageStatus): void 
 + getSectionB(): SectionB 
 + getNsopStorageSet(): List<NsopStorageStatus> 
 + setSectionB(sectionB: SectionB): void 
 + setNsopStorageSet(nsopStorageSet: List<NsopStorageStatus>): void 
 + toString(): String 
+-----------------+
