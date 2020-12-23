## Welcome to APIs For Thammasat Developer  https://restapi.tu.ac.th/

### Prepare ###

- Postman : https://www.postman.com/downloads/
 
- [1] Download File Postman : https://github.com/thepnatee/tu_apis_developers

- [2] หรือ Import URL : https://www.getpostman.com/collections/cf0c7d0289f17005822b

- ปล. เมนู Import อยู่ซ้ายบน จะเลือก Upload ไฟล์โยนง่ายๆใช้ [1] จะเอา URL แปะง่ายกว่าใช้ [2]

### Topic ###

- #Authentication (ยืนยันตัวตน)
- #Instructors (ข้อมูลอาจารย์)
- #Student (ข้อมูลนักศึกษา)
- #Employee (ข้อมูลบุคลากร)
- #Master Data (ข้อมูลหลักทั่วไป)

### Structure ###
- Authentication
  Auth
      - https://restapi.tu.ac.th/api/v1/auth/Ad/verify
  log
      - https://restapi.tu.ac.th/api/v1/auth/Log/auth/?status={true or false}
      - https://restapi.tu.ac.th/api/v1/auth/Log/find/?date={YYYY-mm-dd :2019-05-22}
- Instructors
  Info : https://restapi.tu.ac.th/api/v2/profile/Instructors/info/?First_Name_Th={First_Name_Th}
  Report 
      - https://restapi.tu.ac.th/api/v2/report/Instructors/Fac/all
      - https://restapi.tu.ac.th/api/v2/report/Instructors/Fac/find?Faculty_Name_Th={Faculty_Name_Th}
- Student
  Info : https://restapi.tu.ac.th/api/v2/profile/std/info/?id={student id}
  Report 
      - https://restapi.tu.ac.th/api/v2/report/std/Bucket/all * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}
      - https://restapi.tu.ac.th/api/v2/report/std/fac/all * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}
      - https://restapi.tu.ac.th/api/v2/report/std/Gender/info * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}
      - https://restapi.tu.ac.th/api/v2/report/std/Campus/info * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}
      - https://restapi.tu.ac.th/api/v2/report/std/Level/all
      - https://restapi.tu.ac.th/api/v2/report/std/Adyear/all
      - https://restapi.tu.ac.th/api/v2/report/std/Status/all
- Employee
  Info : https://restapi.tu.ac.th/api/v2/profile/emp/info/?username={username} 
         * ?username={username}&displayname_th={displayname_th}&displayname_en={displayname_en}&organization={organization}
  Report 
      - https://restapi.tu.ac.th/api/v2/emp/org/all * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}
      - https://restapi.tu.ac.th/api/v2/emp/dep/all * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}
      - https://restapi.tu.ac.th/api/v1/report/emp/org/all?Organization={Organization}
- Master Data
      - ข้อมูลจังหวัด อำเภอ ตำบล : https://restapi.tu.ac.th/api/v2/master/Location/map_thai/
      - ตำแหน่งวิชาการ : https://restapi.tu.ac.th/api/v2/master/jobwork/all * กรณีค้นหา /all เปลี่ยนเป็น /find?{ชื่อ field}


เป็นเพียงตัวอย่างเท่านั้นเพิ่มเติมได้ที่ https://restapi.tu.ac.th/
ติดตามข่าวสาร Update หรือตัว รายงานได้ที่ https://lin.ee/AN7L3NO


Source API By : supakarn pradujkanchana @ICT TU API Developer
      
