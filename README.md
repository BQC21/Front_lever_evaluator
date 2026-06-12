# Front_lever_evaluator

## Features
1. User upload video, just only the few seconds when athlete is holding the front lever or its variation
2. Generate video with deep learning to compute relevant angles with pose estimation
3. Graph temporal variation on angles and use both to pose clasification (tuck, tuck advance, half and full)
4. Option to visualize logs table with options to edit and trash

## Stack
1. Next.js: framework to code visualization and browser server functionalities 
2. Fast API: framework to code python functionalities to generate video and analyze graphs
3. MediaPipe: library to pose estimation functionalities
4. Supabase: Database deployment
5. GPT-4o API: generate text notes to analyze graphs

## Database Schema

#### Main Table
- `id` (UUID, Primary Key)
- `back_posterior_angle_avg`
- `posterior_calf_angle_avg`
- `class`
- `time_length`
- `video_file`

...
- `createdAt` (DateTime)
- `updatedAt` (DateTime)
