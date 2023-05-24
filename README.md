---------------------------------
     NsopStorageStatus         
---------------------------------
 - id: Long                    
 - storageStatus: StorageIssues
 - name: StorageNames          
 - status: Status              
---------------------------------
 + NsopStorageStatus()         
 + NsopStorageStatus(          
     name: StorageNames,       
     status: Status            
   )                           
 + addStorageStatus(           
     storageStatus: StorageIssues 
   )                           
 + getId(): Long                
 + getStorageStatus(): StorageIssues 
 + getName(): StorageNames      
 + getStatus(): Status          
 + setId(id: Long)              
 + setStorageStatus(storageStatus: StorageIssues) 
 + setName(name: StorageNames)  
 + setStatus(status: Status)    
 + toString(): String           
---------------------------------



---------------------------------
         ParallelChain          
---------------------------------
 - sectionC: SectionC          
 - issue: String               
---------------------------------
 + ParallelChain()             
 + ParallelChain(               
     name: Names,              
     status: Status,           
     issue: String             
   )                           
 + addSectionC(sectionC: SectionC) 
 + toString(): String           
 + getSectionC(): SectionC     
 + getIssue(): String           
 + setSectionC(sectionC: SectionC) 
 + setIssue(issue: String)      
---------------------------------


---------------------------------
        SchemacsHealth          
---------------------------------
 - sectionD: SectionD          
---------------------------------
 + SchemacsHealth()            
 + SchemacsHealth(              
     name: Names,              
     status: Status,           
     issues: String            
   )                           
 + addSectionD(sectionD: SectionD) 
 + toString(): String           
 + getSectionD(): SectionD     
 + setSectionD(sectionD: SectionD) 
---------------------------------



+-----------------------+
       SectionA        
+-----------------------+
 - id: Long            
 - communicationStatus: CommunicationIssue 
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + SectionA()          
 + SectionA(communicationStatus: CommunicationIssue) 
 + getId(): Long       
 + getCommunicationStatus(): CommunicationIssue 
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setId(id: Long)     
 + setCommunicationStatus(communicationStatus: CommunicationIssue) 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
 + addCommunicationStatus(communicationIssue: CommunicationIssue) 
 + toString(): String  
+-----------------------+



+-----------------------+
       SectionB        
+-----------------------+
 - storageStatus: StorageIssues 
 - standardFileStatus: StandardFileStatus 
 - archivalList: List<NavigationArchival> 
 - uereMeasurementsABlr: List<Uere> 
 - uereMeasurementsBBlr: List<Uere> 
 - uereMeasurementsALck: List<Uere> 
 - uereMeasurementsBLck: List<Uere> 
 - userPositionMeasurements: List<UserPosition> 
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + SectionB(storageStatus: StorageIssues, standardFileStatus: StandardFileStatus, navigationArchivals: List<NavigationArchival>, uereMeasurements: List<Uere>, userPositionMeasurements: List<UserPosition>, issues: String) 
 + getStorageStatus(): StorageIssues 
 + getStandardFileStatus(): StandardFileStatus 
 + getArchivalList(): List<NavigationArchival> 
 + getUereMeasurementsABlr(): List<Uere> 
 + getUereMeasurementsBBlr(): List<Uere> 
 + getUereMeasurementsALck(): List<Uere> 
 + getUereMeasurementsBLck(): List<Uere> 
 + getUserPositionMeasurements(): List<UserPosition> 
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setStorageStatus(storageStatus: StorageIssues) 
 + setStandardFileStatus(standardFileStatus: StandardFileStatus) 
 + setArchivalList(archivalList: List<NavigationArchival>) 
 + setUereMeasurementsABlr(uereMeasurementsABlr: List<Uere>) 
 + setUereMeasurementsBBlr(uereMeasurementsBBlr: List<Uere>) 
 + setUereMeasurementsALck(uereMeasurementsALck: List<Uere>) 
 + setUereMeasurementsBLck(uereMeasurementsBLck: List<Uere>) 
 + setUserPositionMeasurements(userPositionMeasurements: List<UserPosition>) 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
 + addStorageStatus(storageStatus: StorageIssues) 
 + addNavigationArchival(navigationArchival: NavigationArchival) 
 + addUereABlr(uere: Uere) 
 + addUereBBlr(uere: Uere) 
 + addUereALck(uere: Uere) 
 + addUereBLck(uere: Uere) 
 + addUserPositionMeasurement(userPosition: UserPosition) 
 + toString(): String  
+-----------------------+

  
  
  
  +-----------------------+
       SectionC        
+-----------------------+
 - performStandardsFile: PerformanceStandards 
 - performAdvisory: PerformanceAdvisory 
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + SectionC(performStandardsFile: PerformanceStandards, performAdvisory: PerformanceAdvisory, navicPerformanceDetails: NavicPerformanceDetails) 
 + getPerformStandardsFile(): PerformanceStandards 
 + getPerformAdvisory(): PerformanceAdvisory 
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setPerformStandardsFile(performStandardsFile: PerformanceStandards) 
 + setPerformAdvisory(performAdvisory: PerformanceAdvisory) 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
 + toString(): String  
+-----------------------+

  
  +-----------------------+
        SectionD       
+-----------------------+
 - schemacsHealths: List<SchemacsHealth> 
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + SectionD(schemacsHealths: List<SchemacsHealth>, issues: String) 
 + addSchemacsHealth(schemacsHealth: SchemacsHealth) 
 + toString(): String  
 + getSchemacsHealths(): List<SchemacsHealth> 
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setSchemacsHealths(schemacsHealths: List<SchemacsHealth>) 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
+-----------------------+

  
  
  +-----------------------+
        SectionE       
+-----------------------+
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + toString(): String  
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
+-----------------------+

  
  +-----------------------+
        SectionF       
+-----------------------+
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + toString(): String  
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
+-----------------------+

  
  +-----------------------+
        SectionG       
+-----------------------+
 - id: Long            
 - syslogStatus: SyslogStatus 
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + SectionG(syslogStatus: SyslogStatus) 
 + addSysLog(syslogStatus: SyslogStatus) 
 + setId(id: Long)     
 + setSyslogStatus(syslogStatus: SyslogStatus) 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
 + getId(): Long       
 + getSyslogStatus(): SyslogStatus 
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
+-----------------------+

  
  +-----------------------+
        SectionH       
+-----------------------+
 - stnLookAngles: List<StnLookAngle> 
 - navicPerformanceDetails: NavicPerformanceDetails 
+-----------------------+
 + SectionH(issuesFromSectionH: String, stnLookAngles: List<StnLookAngle>) 
 + addStnLookAngle(stnLookAngle: StnLookAngle) 
 + toString(): String  
 + getStnLookAngles(): List<StnLookAngle> 
 + getNavicPerformanceDetails(): NavicPerformanceDetails 
 + setStnLookAngles(stnLookAngles: List<StnLookAngle>) 
 + setNavicPerformanceDetails(navicPerformanceDetails: NavicPerformanceDetails) 
+-----------------------+
