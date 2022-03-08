using System;
using System.IO;
using System.Security.Cryptography;

public class FileIdentificationWithRecursion
{
    static void Main()
    {
        static void WalkDirectoryTree(System.IO.DirectoryInfo root)
        {
            System.IO.FileInfo[] files = null;
            System.IO.DirectoryInfo[] subDirs = null;

            private static readonly Dictionary<string, List<byte[]>> _fileSignature = new Dictionary<string, List<byte[]>>
            { ".zip", new List<byte[]>
            {
                new byte[] { 0x50, 0x4B, 0x03, 0x04}
            }
            },
            { ".jpg", new List<byte[]>
            {
                new byte[] { 0xFF, 0xD8, 0xFF, 0xE0 },
                new byte[] { 0xFF, 0xD8, 0xFF, 0xE1 },
                new byte[] { 0xFF, 0xD8, 0xFF, 0xE8 }
            }
            },
            { ".pdf", new List<byte[]>
            {
                new byte[] { 0x25, 0x50, 0x44, 0x46 }
            }
            }

private static bool IsValidFileExtensionAndSignature(string fileName, Stream data, string[] permittedExtensions)
        {
if (string.IsNullOrEmpty(fileName) || data == null || data.Length == 0)
    foreach (System.IO.FileInfo fi in files)
        {
            return false;
        }
var ext = Path.GetExtension(fileName).ToLowerInvariant();
if (string.IsNullOrEmpty(ext) || !permittedExtensions.Contains(ext))
    foreach (System.IO.FileInfo fi in files)
        {
            return false;
        }
data.Position = 0;
using (var reader = new BinaryReader(data))
            {
if (ext.Equals(".pdf") || ext.Equals(".jpg"))
                {
if (_allowedChars.Length == 0)
                    {

for (var i = 0; i < data.Length; i++)
                        {
if (reader.ReadByte() > sbyte.MaxValue)
                            {
return false;
                            }
                        }
                    }
else
                    {
for (var i = 0; i < data.Length; i++)
                        {
var b = reader.ReadByte();
if (b > sbyte.MaxValue ||
!_allowedChars.Contains(b))
                            {
return false;
                            }
                        }
                    }
return true;
                }
var signatures = _fileSignature[ext];
var headerBytes = reader.ReadBytes(signatures.Max(m => m.Length));
return signatures.Any(signature => 
headerBytes.Take(signature.Length).SequenceEqual(signature));
            }
        }
if (string.IsValidFileExtensionAndSignature(fileName) && ext.Equals(".pdf")
    using (SHA256 mySHA256 = SHA256.Create())
    {
        foreach (FileInfo fInfo in files)
                {
                    using (FileStream fileStream = fInfo.Open(FileMode.Open))
                    {
                        try
                        {
                            fileStream.Position = 0;
                            byte[] hashValue = mySHA256.ComputeHash(fileStream);
                            Console.Write($"{fInfo.Name}: ");
                            PrintByteArray(hashValue);
                        }
                        catch (IOException e)
                        {
                            Console.WriteLine($"I/O Exception: {e.Message}");
                        }
                        catch (UnauthorizedAccessException e)
                        {
                            Console.WriteLine($"Access Exception: {e.Message}");
                        }
                    }
                }
            }
        }
        else
        {
            Console.WriteLine("The directory specified could not be found.");
        }
    }

    foreach (System.IO.FileInfo fi in files)
        {
            string[] pdfFiles =
            {
                $"{fileName} {hashvalue}"
            };
        };
if (string.IsValidFileExtensionAndSignature(fileName) && ext.Equals(".jpg")
using (SHA256 mySHA256 = SHA256.Create())
    {
        foreach (FileInfo fInfo in files)
                {
                    using (FileStream fileStream = fInfo.Open(FileMode.Open))
                    {
                        try
                        {
                            fileStream.Position = 0;
                            byte[] hashValue = mySHA256.ComputeHash(fileStream);
                            Console.Write($"{fInfo.Name}: ");
                            PrintByteArray(hashValue);
                        }
                        catch (IOException e)
                        {
                            Console.WriteLine($"I/O Exception: {e.Message}");
                        }
                        catch (UnauthorizedAccessException e)
                        {
                            Console.WriteLine($"Access Exception: {e.Message}");
                        }
                    }
                }
            }
        }
        else
        {
            Console.WriteLine("The directory specified could not be found.");
        }
    }

    foreach (System.IO.FileInfo fi in files)
        {
            string[] jpgFiles =
            {
                $"{fileName} {hashvalue}"
            };
        };
DirectoryInfo dataDir = new DirectoryInfo(@"C:\Users\example\signaturedata")
string csvFilePath = @"C:\Users\example\signaturedata\sample1.csv";

    File.WriteAllLines(csvFilePath, pdfFiles);
    File.WriteAllLines(csvFilePath, jpgFiles);

        foreach(string f in File.ReadAllLines(csvFilePath))
            {
                Console.WriteLine($"File types and path: {f}");
            }

            Concole.ReadLine();

subDirs = root.GetDirectories();

    foreach (System.IO.DirectoryInfo dirInfo in subDirs)
        {
            WalkDirectoryTree(dirInfo);
        }

           
        }
    }
}
