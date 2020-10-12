import os, shutil

origin = ['desktop.ini', 'Paulo']
actual = os.listdir("C:/Users/55839/Desktop")
filesToBeMoved = []

for file in actual:
    if file not in origin:
        filesToBeMoved.append(file)

def ext(file):
    splited = file.split(".")
    extension = splited[-1]
    
    if extension != file:
        return extension
    else:
        return ""

extensions = {
    #media
        #audio
    "aif" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "cda" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "mid" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "midi": "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "mp3" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "mpa" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "ogg" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "wav" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "wma" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
    "wpl" : "C:/Users/55839/Desktop/Paulo/Media/Audio",
        #images
    "ai"  : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "bmp" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "gif" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "ico" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "jpeg": "C:/Users/55839/Desktop/Paulo/Media/Images",
    "jpg" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "png" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "ps"  : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "psd" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "svg" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "tif" : "C:/Users/55839/Desktop/Paulo/Media/Images",
    "tiff": "C:/Users/55839/Desktop/Paulo/Media/Images",
        #video
    "avi" : "C:/Users/55839/Desktop/Paulo/Media/Videos",
    "mkv" : "C:/Users/55839/Desktop/Paulo/Media/Videos",
    "mp4" : "C:/Users/55839/Desktop/Paulo/Media/Videos",
    "mpg" : "C:/Users/55839/Desktop/Paulo/Media/Videos",
    "mpeg": "C:/Users/55839/Desktop/Paulo/Media/Videos",
    "wmv" : "C:/Users/55839/Desktop/Paulo/Media/Videos",
    #scipts
        #programming
    "py" : "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "rb" : "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "js" : "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "nim": "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "dart":"C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "cp" : "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "c"  : "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
    "css": "C:/Users/55839/Desktop/Paulo/Scripts/Programming",
        #executables
    "apk" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "bin" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "bat" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "exe" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "cmd" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "dll" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "ini" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "sys" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
    "tmp" : "C:/Users/55839/Desktop/Paulo/Scripts/Executables",
        #shortcuts
    "lnk" : "C:/Users/55839/Desktop/Paulo/Scripts/Shortcuts",
    #text
        #textfiles
    "txt" : "C:/Users/55839/Desktop/Paulo/Text/TextFiles",
    "log" : "C:/Users/55839/Desktop/Paulo/Text/TextFiles",
        #docs
    "pdf" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "odt" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "md"  : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "xls" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "ods" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "odp" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "ppt" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "pptx": "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "doc" : "C:/Users/55839/Desktop/Paulo/Text/Docs",
    "docs": "C:/Users/55839/Desktop/Paulo/Text/Docs",
    #web
    "html": "C:/Users/55839/Desktop/Paulo/Web",
    "htm" : "C:/Users/55839/Desktop/Paulo/Web",
    "xml" : "C:/Users/55839/Desktop/Paulo/Web",
    #other
        #und
    "" : "C:/Users/55839/Desktop/Paulo/Other/Undefined",
        #compact
    "zip" : "C:/Users/55839/Desktop/Paulo/Other/Compact",
    "rar" : "C:/Users/55839/Desktop/Paulo/Other/Compact",
    "rpm" : "C:/Users/55839/Desktop/Paulo/Other/Compact",
    "pkg" : "C:/Users/55839/Desktop/Paulo/Other/Compact"
}

for file in filesToBeMoved:
    fileExt = ext(file)
    try:
        shutil.move("C:/Users/55839/Desktop/" + file, extensions[fileExt] + "/" + file)
    except KeyError:
        shutil.move("C:/Users/55839/Desktop/" + file, "C:/Users/55839/Desktop/Paulo/Other/Undefined/" + file)