## Laravel: Using One pivot table id in another pivot table

I'm working in a Laravel 7 project. I've implemented my table structure as below:

Classes and Sections many-to-many

#### classes

    name

#### sections

    name

#### class_section

    class_id
    section_id

Teachers and Subjects many-to-many

#### teachers

    name
    email
    designation

#### subjects

    name

#### subject_teacher

    subject_id
    teacher_id

Now, what i want is to use the `class_section` (pivot) `id` inside `subject_teacher` pivot table, so that i can insert the `class_section_id` in `subject_teacher` table and get the class/section of specific teacher/subject.

Any idea how to do this using `Laravel Eloquent` ?
