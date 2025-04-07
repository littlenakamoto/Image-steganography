# Image Steganography Tool

## What is Image Steganography?

Image Steganography is the art and science of concealing secret information within an image, cleverly tucked away so the human eye can’t spot a difference. The term "steganography" comes from Greek, meaning "covered writing"—think of it as a digital sleight of hand. Unlike encryption, which scrambles your message into an unreadable jumble, steganography hides it in plain sight, blending it seamlessly into the pixels of an innocent-looking picture.

This tool uses a sophisticated method to embed your data into the least significant bits (LSB) of an image’s pixel values, ensuring the changes are imperceptible. Paired with military-grade AES-256 encryption, your secrets stay locked tight—accessible only with the right password.

## How It Works

- **Hiding**: Enter your secret message (like a Bitcoin seed or password), choose an image, and set a password. The tool encrypts your message with AES-256, converts it to binary, and embeds it into the image. If the image is too small, it scales proportionally to fit the data—keeping the aspect ratio intact for a natural look.
- **Revealing**: Upload the modified image, input the password, and the tool extracts and decrypts the hidden message. Simple, secure, and sneaky.

## Features

- **Dynamic Scaling**: Images automatically resize (proportionally!) to accommodate your message, so no awkward white patches or distorted stretches.
- **AES-256 Encryption**: Your data gets wrapped in top-tier encryption before hiding, with a unique salt and IV for each use.
- **User-Friendly**: Clean interface, dark mode toggle, and a one-click download for your stego-image.

## Legal Notice

**⚠️ IMPORTANT: This tool is designed *exclusively* for legitimate, lawful purposes—think securing Bitcoin seeds, private keys, or personal passwords. Any use for illegal activities (e.g., concealing malicious code, evading authorities, or breaking laws) is strictly prohibited.** Misuse could land you in serious trouble with agencies like the CIA, FBI, or local law enforcement. The creator of this tool bears **no responsibility** for unlawful actions taken by users. Use it wisely, ethically, and legally—or don’t use it at all.

## Technical Bits (For the Curious)

- **LSB Embedding**: The message is hidden in the least significant bit of the red channel in the last row of pixels. Each pixel can store one bit, so a 1424-pixel-wide row can hold 1424 bits.
- **Proportional Scaling**: If your message needs more pixels than the image provides, it scales up based on the original aspect ratio (e.g., a 1024x768 image needing 1424 pixels becomes 1424x1068).
- **Crypto Strength**: AES-256 with PBKDF2 key derivation (30,000 iterations) ensures brute-forcing the password is a nightmare for attackers.

## Why Use It?

Perfect for anyone needing to stash sensitive data discreetly—like crypto enthusiasts protecting their wallet seeds or privacy buffs safeguarding secrets. It’s a blend of stealth and security, wrapped in a sleek package.

**Reminder**: Keep it legal, keep it safe, and enjoy the magic of hidden messages!
