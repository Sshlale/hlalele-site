export default {
  async fetch(request, env) {
    if (request.method === "POST") {
      const formData = await request.formData();
      const email = formData.get("email");
      if (email) {
        await env.NEWSLETTER.put(email, "subscribed");
        return new Response("✨ Inscribed successfully!", { status: 200 });
      }
    }
    return new Response("Invalid request", { status: 400 });
  }
};
