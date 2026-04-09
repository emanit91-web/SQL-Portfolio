CREATE TABLE claims_data (
    claim_id INTEGER PRIMARY KEY,
    member_id INTEGER,
    provider_id INTEGER,
    claim_type TEXT,
    service_date TEXT,
    diagnosis_code TEXT,
    procedure_code TEXT,
    billed_amount REAL,
    paid_amount REAL,
    claim_status TEXT,
    plan_type TEXT
);
INSERT INTO claims_data VALUES
(1,1001,501,'Medical','2025-01-05','E11.9','99213',250,180,'Paid','Commercial'),
(2,1002,502,'Pharmacy','2025-01-18','I10','RX001',120,95,'Paid','Medicare'),
(3,1003,503,'Medical','2025-02-03','J45.909','93000',400,0,'Denied','Medicaid'),
(4,1004,501,'Medical','2025-02-12','E78.5','80061',180,130,'Paid','Commercial'),
(5,1005,504,'Pharmacy','2025-02-26','E11.9','RX002',300,240,'Paid','Commercial'),
(6,1006,505,'Medical','2025-03-09','M54.5','72100',500,350,'Paid','Medicare'),
(7,1007,503,'Medical','2025-03-21','I10','99214',275,0,'Denied','Medicaid'),
(8,1008,502,'Pharmacy','2025-04-02','E78.5','RX003',90,75,'Paid','Commercial'),
(9,1009,504,'Medical','2025-04-15','E11.9','83036',150,110,'Paid','Commercial'),
(10,1010,505,'Medical','2025-04-29','J45.909','94010',325,250,'Paid','Medicare'),
(11,1011,506,'Pharmacy','2025-05-08','I10','RX001',115,90,'Paid','Medicaid'),
(12,1012,501,'Medical','2025-05-19','E78.5','99213',225,175,'Paid','Commercial'),
(13,1013,507,'Medical','2025-06-04','M54.5','97110',600,0,'Denied','Commercial'),
(14,1014,508,'Pharmacy','2025-06-17','E11.9','RX004',210,165,'Paid','Medicare'),
(15,1015,503,'Medical','2025-06-28',NULL,'99214',310,220,'Paid','Medicaid'),
(16,1016,504,'Pharmacy','2025-07-10','I10','RX002',130,105,'Paid','Commercial'),
(17,1017,509,'Medical','2025-07-22','E11.9','80053',275,200,'Paid','Commercial'),
(18,1018,510,'Medical','2025-08-06','J45.909','99213',260,0,'Denied','Medicare'),
(19,1019,507,'Pharmacy','2025-08-19','E78.5','RX003',95,80,'Paid','Medicaid'),
(20,1020,506,'Medical','2025-09-03','I10','93000',420,300,'Paid','Commercial');
SELECT *FROM claims_data;
SELECT claim_status, COUNT(*)
FROM claims_data
GROUP BY claim_status;
SELECT claim_type, sum(paid_amount)
FROM claims_data
GROUP by claim_type;
SELECT plan_type, avg(paid_amount)
from claims_data
group by plan_type;
SELECT *
FROM claims_data
where claim_status = 'Denied';
SELECT diagnosis_code, sum(paid_amount)
from claims_data
group by diagnosis_code
order by sum(paid_amount) DESC;
SELECT * FROM claims_data;

