# ACL Configuration

## Goal
Restrict Medicine-related course files so only "career.coach.one" can access them.

## ACL File (acl.json)
Stored at:
s3://career4all-course-catalog-anandsr/security/course_access_acl_coach.json

ACL rules:
- ALLOW: career.coach.one
- DENY: career.coach.two

ACL format uses USER-level entries because creating new groups is not permitted.

## Verification
### User: career.coach.one
- Can see restricted medical courses.
- Screenshot: acl-allow.png

### User: career.coach.two
- Cannot see restricted courses.
- Screenshot: acl-deny.png
