<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>File Upload Manager</title>
<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: "Poppins", sans-serif;
    }

    body {
        background: linear-gradient(135deg, #667eea, #764ba2);
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .upload-container {
        background: #fff;
        padding: 30px;
        border-radius: 15px;
        width: 400px;
        box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        text-align: center;
    }

    h2 {
        color: #333;
        margin-bottom: 20px;
    }

    .upload-box {
        border: 2px dashed #667eea;
        border-radius: 10px;
        padding: 30px;
        cursor: pointer;
        transition: all 0.3s ease;
    }

    .upload-box:hover {
        background-color: #f8f8ff;
        border-color: #764ba2;
    }

    .upload-box input[type="file"] {
        display: none;
    }

    .upload-box label {
        display: block;
        color: #555;
        font-weight: 500;
    }

    .file-list {
        margin-top: 20px;
        text-align: left;
        max-height: 150px;
        overflow-y: auto;
        border-top: 1px solid #eee;
        padding-top: 10px;
    }

    .file-list li {
        padding: 8px 10px;
        background: #f9f9f9;
        border-radius: 5px;
        margin-bottom: 8px;
        font-size: 14px;
        color: #333;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .file-list li span {
        color: #999;
        font-size: 12px;
    }

    .btn {
        margin-top: 20px;
        background: #667eea;
        color: #fff;
        padding: 10px 20px;
        border: none;
        border-radius: 8px;
        cursor: pointer;
        transition: 0.3s;
    }

    .btn:hover {
        background: #764ba2;
    }
</style>
</head>
<body>

<div class="upload-container">
    <h2>File Upload Manager</h2>

    <div class="upload-box">
        <input type="file" id="fileUpload" multiple>
        <label for="fileUpload">Click or Drag Files Here to Upload</label>
    </div>

    <ul class="file-list">
        <li>example_file1.pdf <span>2.4 MB</span></li>
        <li>photo_image.png <span>1.1 MB</span></li>
        <li>project_doc.docx <span>850 KB</span></li>
    </ul>

    <button class="btn">Upload Files</button>
</div>

</body>
</html>
