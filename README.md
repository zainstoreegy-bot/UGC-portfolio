# UGC-portfolio
import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Mail, Instagram, Camera, User, CheckCircle, Star } from "lucide-react";

export default function UGCPortfolio() { return ( <div className="min-h-screen bg-white text-gray-900 p-6 font-sans"> <header className="text-center mb-12"> <h1 className="text-4xl font-bold mb-2">Hi, I'm Mariam</h1> <p className="text-lg">UGC Creator | Product Photographer | Content Strategist</p> </header>

<section className="max-w-4xl mx-auto mb-12 text-center">
    <h2 className="text-2xl font-bold mb-2 flex items-center justify-center gap-2">
      <User size={20} /> About Me
    </h2>
    <p className="text-gray-700">
      I'm a 19-year-old UGC creator based in Egypt. I specialize in product photography and creating relatable, aesthetic, and conversion-focused content for brands. With a strong passion for visual storytelling and digital marketing, I help brands connect authentically with their audience.
    </p>
  </section>

  <section className="max-w-4xl mx-auto mb-12 text-center">
    <h2 className="text-2xl font-bold mb-2 flex items-center justify-center gap-2">
      <CheckCircle size={20} /> My Services
    </h2>
    <ul className="text-gray-700 list-disc list-inside text-left max-w-md mx-auto">
      <li>UGC Video Creation (TikTok & Reels)</li>
      <li>Product Photography for E-commerce & Social Media</li>
      <li>Unboxing & Testimonial Videos</li>
      <li>Scriptwriting for Ad Creatives</li>
      <li>Voiceover & POV Style Content</li>
    </ul>
  </section>

  <section className="max-w-6xl mx-auto mb-12">
    <h2 className="text-2xl font-bold mb-6 text-center">My Portfolio</h2>
    <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
      {[1, 2, 3, 4, 5, 6].map((item) => (
        <Card key={item} className="rounded-2xl shadow-md overflow-hidden">
          <CardContent className="p-0">
            <img
              src={`https://source.unsplash.com/600x400/?product,ugc,photography&sig=${item}`}
              alt="UGC Work Sample"
              className="w-full h-64 object-cover"
            />
            <div className="p-4">
              <h2 className="text-xl font-semibold">Project Title</h2>
              <p className="text-sm text-gray-600 mt-1">
                Short description about the UGC content, platform, or client.
              </p>
            </div>
          </CardContent>
        </Card>
      ))}
    </div>
  </section>

  <section className="max-w-4xl mx-auto mb-12 text-center">
    <h2 className="text-2xl font-bold mb-4 flex items-center justify-center gap-2">
      <Star size={20} /> Client Testimonials
    </h2>
    <div className="grid md:grid-cols-2 gap-6">
      <div className="bg-gray-50 rounded-xl p-6 shadow-sm">
        <p className="text-gray-700 italic">
          “Working with Mariam was a breeze! She delivered exactly what we asked for and more. The content looked amazing and matched our brand’s voice perfectly.”
        </p>
        <p className="mt-4 font-semibold">— Nour Cosmetics</p>
      </div>
      <div className="bg-gray-50 rounded-xl p-6 shadow-sm">
        <p className="text-gray-700 italic">
          “Highly professional, creative, and easy to communicate with. I’ll definitely collaborate with her again!”
        </p>
        <p className="mt-4 font-semibold">— Zayn Home Decor</p>
      </div>
    </div>
  </section>

  <section className="mt-12 text-center">
    <h2 className="text-2xl font-bold mb-4">Let’s Work Together!</h2>
    <p className="text-gray-600 mb-6">
      I'm open to collaborations and brand deals. Let’s create engaging content that speaks to your audience.
    </p>
    <div className="flex flex-wrap justify-center gap-4">
      <Button variant="outline" className="flex gap-2 items-center">
        <Instagram size={16} /> @ugc.by.egyptian.g
      </Button>
      <Button variant="outline" className="flex gap-2 items-center">
        <Mail size={16} /> ugc.mariam@email.com
      </Button>
      <Button variant="default" className="flex gap-2 items-center">
        <Camera size={16} /> View More Work
      </Button>
    </div>
  </section>
</div>

); }

