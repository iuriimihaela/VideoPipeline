# Video Pipeline Lab with Kafka, S3, and FFmpeg

This project implements a video pipeline using Kafka for stream processing, S3 for storage, and `ffmpeg` for video conversion into multiple formats. Using TypeScript and Node.js, this pipeline enables downloading, processing, and saving video files in various formats.

## Description

The goal of this lab is to create a video pipeline that:
1. **Downloads video files** using a tool like `yt-dlp`.
2. **Stores video files on S3**.
3. **Processes video files** using `ffmpeg` to convert them into multiple formats.
4. **Uses Kafka** to transmit messages between different parts of the system.

## Technologies Used

- **TypeScript**: The primary programming language.
- **Node.js**: The runtime platform for the application.
- **Kafka**: A messaging system for parallel processing of files.
- **S3**: A storage service for video files.
- **ffmpeg**: A video processing tool used for file conversion.
- **yt-dlp**: A tool for downloading videos from various platforms.

## Installation

To run this project on your local machine, follow these steps:

### 1. Clone the Repository

Clone the repository to your desired directory:

```bash
git clone <REPO-URL>
cd <project-directory>
```
### 2. Install Dependencies
Install all necessary dependencies using npm or yarn:

```bash
npm install ...
```
# or
```bash
yarn install ...
```
### 3. Configure Kafka and S3
Ensure that Kafka and S3 are properly configured. Modify the configuration file to include your S3 and Kafka authentication details.

### 4. Install yt-dlp and ffmpeg
To download and process video files, you need to install the following:

yt-dlp: Installation instructions for yt-dlp
ffmpeg: Installation instructions for ffmpeg
After installation, ensure that both tools are available in your system's PATH.

### 5. Run the Application
Once all dependencies and configurations are set up, start the application by running:

# Run the producer to download the videos

```bash
ts-node videoPipeline.ts producer
```
# Run the consumer to do the conversions 

```bash
ts-node videoPipeline.ts consumer
```
