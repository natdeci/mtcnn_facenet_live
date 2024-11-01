# Face Recognition Using MTCNN and Facenet
This project is intended for live attendance by detecting faces to verify people's appearance.

The detection model used is MTCNN, that is excellent in detecting even small faces in an image. Though it may not be fast, its ability is required due to usage of cctv for monitoring people.

The face recognition model used is FaceNet from Google. The model is designed to be deployed on edge device, ensuring its speed.

----------------------------------------------------------------------

The directory in the main branch is simply a folder with many images, the file name for the images must be the name of that person.

The directory's structure in the 'new-structure-branch' branch is having a folder consisting of many other folders for each person. Each person would have multiple images of reference, prefferably augmented so the model could detect the faces even in bad lighting, different angles, and moving targets.

----------------------------------------------------------------------

Files would be loaded into a dictionary with the people's name as the key, and each key's value is a list, a list consisting of embeddings for that person reference images.