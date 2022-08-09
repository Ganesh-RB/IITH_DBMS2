# Database Design

Here we developed a PostgreSQL database from raw erroneous data. 

## Java Files
- [Schema.java](Schema.java) creates a Database with JDBC and defines a schema for it.
- [parser_and_loader.java](parser_and_loader.java) parses the data from [Source file](https://drive.google.com/file/d/12bMEkZwF0eYD9j5GU_Ft-r8gAyYNEHYx/view?usp=sharing) and store it into database.

## For data correction we applied following methods.
- Convert author's name to lower case and stored in HashMap for eliminating duplicates in name.
- Similarly stored venue in HashMap and stored same in Vector container and then in database.
- We choose HashMap as it allow to store author Name and its id in one container, and also it allows a null value if required.
- Stored details of paper, author and venues in Vector container and stored same into database.


## CSV Files for created database are
- [Author](https://drive.google.com/file/d/1hKxWAKtYr9CYqex4shxUD_3iA_Beske0/view?usp=sharing)
- [Citation](https://drive.google.com/file/d/1j33qP6hujL3pVP7vWg-jQOfWyb_C2NaP/view?usp=sharing)
- [Conference](https://drive.google.com/file/d/1tinhIIWBvh0jUt01VEm_Py1aa35ESsC7/view?usp=sharing)
- [Research Paper](https://drive.google.com/file/d/1vPhgPviJ-HcBXJDiEDiigLQyi_jAXeTc/view?usp=sharing)
- [Written By](https://drive.google.com/file/d/1RLIAuycyQmRuhHv9wdEH5DZTToQ1XlMN/view?usp=sharing)

**Note:** Final database dump file can be viewed [here](https://drive.google.com/file/d/1q14Eb8ChQCw1x8BZJGTW82BP-sIbw2Qi/view?usp=sharing)